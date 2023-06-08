<template>
  <div class="card">
    <div class="card__side card__side--front" :class="'card__side--front-' + styleModifier">
      <div class="card__picture u-margin-bottom-medium" :class="'card__picture--' + styleModifier">
        &nbsp;
      </div>
      <h4 class="card__title">
        <span :class="'card__title--' + styleModifier">{{ title }}</span>
      </h4>
      <div class="card__content">
        <ul>
            <li v-for="content in contentList" :key="content">{{ content }}</li>
        </ul>
      </div>
    </div>
    <div class="card__side card__side--back" :class="'card__side--back-' + styleModifier">
      <div class="card__price-box">
        <div class="card__price-info u-margin-bottom-large">
          <p>Only</p>
          <p>$ {{ price }}</p>
        </div>
        <a href="#" class="btn btn--white">Book Now!</a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
    props: {
        title : String,
        contentList: Array,
        price: Number,
        styleModifier: Number
    }
}
</script>