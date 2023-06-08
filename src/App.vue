<template>
  <div class="container">
    <div class="navigation">
      <input
        type="checkbox"
        class="navigation__checkbox"
        id="navigation__menu"
        hidden
      />
      <label for="navigation__menu" class="navigation__button">
        <span class="navigation__icon"></span>
      </label>

      <div class="navigation__background">&nbsp;</div>

      <div class="navigation__content">
        <ul class="navigation__list">
          <li class="navigation__item">
            <a href="#" class="navigation__link"
              ><span>01</span>About natours</a
            >
          </li>
          <li class="navigation__item">
            <a href="#" class="navigation__link"
              ><span>02</span>Your benefits</a
            >
          </li>
          <li class="navigation__item">
            <a href="#" class="navigation__link"
              ><span>03</span>Popular tours</a
            >
          </li>
          <li class="navigation__item">
            <a href="#" class="navigation__link"><span>04</span>Stories</a>
          </li>
          <li class="navigation__item">
            <a href="#" class="navigation__link"><span>05</span>Book now</a>
          </li>
        </ul>
      </div>
    </div>
    <header class="header">
      <div class="header__logo-box">
        <img
          class="header__logo"
          src="./assets/img/logo-white.png"
          alt="Logo"
        />
      </div>
      <div class="header__text-box">
        <h1 class="heading-primary">
          <span class="heading-primary--main">Outdoors</span>
          <span class="heading-primary--sub">is where life happens</span>
        </h1>
        <a href="#" class="btn btn--white btn--animate">Discover our tours</a>
      </div>
    </header>
    <main>
      <section class="section-about">
        <div class="u-text-center u-margin-bottom-large">
          <h2 class="heading-secondary">
            Exciting tours for adventurous people
          </h2>
        </div>
        <div class="row">
          <div class="col-1-of-2">
            <h3 class="heading-tertiary u-margin-bottom-small">
              You're going to fall in love with nature
            </h3>
            <p class="paragraph">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit.
              Perferendis expedita distinctio consectetur quae optio odio porro
              minima vero officiis perspiciatis corporis id assumenda, iusto,
              consequatur atque cum ipsa quibusdam? Blanditiis.
            </p>
            <h3 class="heading-tertiary u-margin-bottom-small">
              Live adventures like you have never before
            </h3>
            <p class="paragraph">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Voluptates aspernatur distinctio omnis laudantium possimus unde.
              Aut, doloribus, neque quaerat voluptatum deleniti repudiandae
              voluptas illo voluptatem ex at quis expedita ducimus?
            </p>
            <a href="#" class="btn-text">Learn More &rarr;</a>
          </div>
          <div class="col-1-of-2">
            <div class="composition">
              <img
                class="composition__photo composition__photo--p1"
                src="./assets/img/nat-1-large.jpg"
                alt="Photo 1"
              />
              <img
                class="composition__photo composition__photo--p2"
                src="./assets/img/nat-2-large.jpg"
                alt="Photo 2"
              />
              <img
                class="composition__photo composition__photo--p3"
                src="./assets/img/nat-3-large.jpg"
                alt="Photo 3"
              />
            </div>
          </div>
        </div>
      </section>
      <section class="section-features">
        <div class="row">
          <div class="col-1-of-4">
            <div class="feature-box">
              <i class="feature-box__icon icon-basic-world"></i>
              <h3 class="heading-tertiary u-margin-bottom-small">
                Explore the world
              </h3>
              <p class="feature-box__text">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Suscipit voluptas explicabo, fugit ab debitis perferendis
              </p>
            </div>
          </div>
          <div class="col-1-of-4">
            <div class="feature-box">
              <i class="feature-box__icon icon-basic-compass"></i>
              <h3 class="heading-tertiary u-margin-bottom-small">
                Meet nature
              </h3>
              <p class="feature-box__text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Reprehenderit accusantium esse magnam suscipit hic. Harum
                repellat consectetur culpa nam
              </p>
            </div>
          </div>
          <div class="col-1-of-4">
            <div class="feature-box">
              <i class="feature-box__icon icon-basic-map"></i>
              <h3 class="heading-tertiary u-margin-bottom-small">
                Find your way
              </h3>
              <p class="feature-box__text">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Unde
                natus doloremque quibusdam quam, minus rerum illum facilis nemo
                magni blanditiis id doloribus similique enim. Molestias natus
              </p>
            </div>
          </div>
          <div class="col-1-of-4">
            <div class="feature-box">
              <i class="feature-box__icon icon-basic-heart"></i>
              <h3 class="heading-tertiary u-margin-bottom-small">
                Live a healthier life
              </h3>
              <p class="feature-box__text">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                Molestias alias veniam voluptates consequuntur quaerat
                voluptatem cumque voluptate. Sunt amet odio voluptates cum
                consequatur tenetur nostrum. Ipsam illum sapiente fuga placeat.
              </p>
            </div>
          </div>
        </div>
      </section>
      <section class="section-tours">
        <div class="u-text-center u-margin-bottom-large">
          <h2 class="heading-secondary">Most popular tours</h2>
        </div>
        <div class="row">
          <div class="col-1-of-3">
            <card-box
              :title="'The sea explorer'"
              :contentList="[
                '3 day tour',
                'Up to 30 people',
                '2 tour guides',
                'Sleep in cozy hostels',
                'Difficulty: very easy',
              ]"
              :price="297"
              :styleModifier="1"
            ></card-box>
          </div>
          <div class="col-1-of-3">
            <card-box
              :title="'The forest hiker'"
              :contentList="[
                '7 day tour',
                'Up to 40 people',
                '6 tour guides',
                'Sleep in provided tents',
                'Difficulty: medium',
              ]"
              :price="497"
              :styleModifier="2"
            >
            </card-box>
          </div>
          <div class="col-1-of-3">
            <card-box
              :title="'The snow adventurer'"
              :contentList="[
                '5 day tours',
                'Up to 15 people',
                '3 tour guides',
                'Sleep in provided tents',
                'Difficulty: hard',
              ]"
              :price="897"
              :styleModifier="3"
            >
            </card-box>
          </div>
        </div>
        <div class="u-text-center u-margin-top-large">
          <a href="#" class="btn btn--green">Discover all tours</a>
        </div>
      </section>
      <section class="section-stories">
        <div class="bg-video">
          <video class="bg-video__content" autoplay muted loop>
            <source src="./assets/img/video.mp4" type="video/mp4" />
            <source src="./assets/img/video.webm" type="video/webm" />
            Your browser is not supported
          </video>
        </div>

        <div class="u-text-center u-margin-bottom-large">
          <h2 class="heading-secondary">We make people genuinely happy</h2>
        </div>
        <div class="row">
          <div class="story">
            <figure class="story__shape">
              <img
                src="./assets/img/nat-8.jpg"
                alt="Person on a tour"
                class="story__img"
              />
              <figcaption class="story__caption">Mary Smith</figcaption>
            </figure>
            <div class="story__text">
              <h3 class="heading-tertiary u-margin-bottom-small">
                I had the best week ever with my family
              </h3>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                Tempore reiciendis saepe accusantium assumenda. Laborum illo
                esse, ex dolores qui ipsam non iusto nesciunt architecto rerum
                aut expedita amet deleniti doloremque. iusto nesciunt architecto
                rerum aut expedita amet deleniti doloremque.
              </p>
            </div>
          </div>
          <div class="story">
            <figure class="story__shape">
              <img
                src="./assets/img/nat-9.jpg"
                alt="Person on a tour"
                class="story__img"
              />
              <figcaption class="story__caption">Jack Wilson</figcaption>
            </figure>
            <div class="story__text">
              <h3 class="heading-tertiary u-margin-bottom-small">
                Wow! my life is completely different now
              </h3>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                Tempore reiciendis saepe accusantium assumenda. Laborum illo
                esse, ex dolores qui ipsam non iusto nesciunt architecto rerum
                aut expedita amet deleniti doloremque. iusto nesciunt architecto
                rerum aut expedita amet deleniti doloremque.
              </p>
            </div>
          </div>
        </div>
        <div class="u-text-center u-margin-top-large">
          <a href="#" class="btn-text">Read all stories &rarr;</a>
        </div>
      </section>
      <section class="section-book">
        <div class="row">
          <div class="book">
            <div class="book__form">
              <div class="u-margin-bottom-medium">
                <h2 class="heading-secondary">Start booking now!</h2>
              </div>
              <form action="#" class="form" @submit.prevent>
                <div class="form__group">
                  <input
                    type="text"
                    class="form__input"
                    placeholder="Full name"
                    id="name"
                    required
                  />
                  <label for="name" class="form__label">Full name</label>
                </div>
                <div class="form__group">
                  <input
                    type="email"
                    class="form__input"
                    placeholder="Email address"
                    id="email"
                    required
                  />
                  <label for="email" class="form__label">Email address</label>
                </div>
                <div class="form__group">
                  <div class="form__radio">
                    <input
                      type="radio"
                      class="form__radio-input"
                      id="small"
                      name="size"
                      hidden
                    />
                    <label for="small" class="form__label">
                      <span class="form__radio-btn"></span>
                      Small tour group
                    </label>
                  </div>
                  <div class="form__radio">
                    <input
                      type="radio"
                      class="form__radio-input"
                      id="large"
                      name="size"
                      hidden
                    />
                    <label for="large" class="form__label">
                      <span class="form__radio-btn"></span>
                      Large tour group
                    </label>
                  </div>
                </div>
                <div class="form__group u-margin-top-medium">
                  <input
                    type="submit"
                    class="btn btn--green"
                    value="Next step &rarr;"
                  />
                </div>
              </form>
            </div>
          </div>
        </div>
      </section>
    </main>
    <footer class="footer">
      <div class="footer__logo-box u-margin-bottom-large">
        <img
          src="./assets/img/logo-green-2x.png"
          alt=""
          class="footer__logo-img"
        />
      </div>
      <div class="row">
        <div class="col-1-of-2">
          <div class="footer__navigation">
            <ul class="footer__list">
              <li class="footer__item">
                <a href="#" class="footer__link">Company</a>
              </li>
              <li class="footer__item">
                <a href="#" class="footer__link">Contact Us</a>
              </li>
              <li class="footer__item">
                <a href="#" class="footer__link">Carrers</a>
              </li>
              <li class="footer__item">
                <a href="#" class="footer__link">Privacy Policy</a>
              </li>
              <li class="footer__item">
                <a href="#" class="footer__link">Terms</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-1-of-2">
          <p class="footer__copyright">
            Built by JONAS SCHMEDTMANN for his online course ADVANCED CSS AND
            SASS. Some of the presented CSS features are highly experimental and
            may not work in all browsers, or may work in a different way at the
            time of watching this video. Web development changes quickly, just
            live with it &#128513;
          </p>
        </div>
      </div>
    </footer>

    <div class="popup">
      <div class="popup__content">
        <div class="popup__left">
          <img src="./assets/img/nat-8.jpg" alt="" class="popup__img" />
          <img src="./assets/img/nat-9.jpg" alt="" class="popup__img" />
        </div>
        <div class="popup__right">
          <h1 class="heading-secondary u-margin-bottom-small">Start Booking Now</h1>
          <h2 class="heading-tertiary u-margin-bottom-small">
            Important - Please read the terms and condition first
          </h2>
          <p class="popup__text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Augue
            mauris augue neque gravida in fermentum et sollicitudin. Arcu risus
            quis varius quam quisque id diam vel quam. Scelerisque eleifend
            donec pretium vulputate sapien. Posuere urna nec tincidunt praesent
            semper feugiat nibh sed. Gravida quis blandit turpis cursus in hac
            habitasse. Odio morbi quis commodo odio aenean sed adipiscing diam
            donec. Cursus risus at ultrices mi. Ornare quam viverra orci
            sagittis eu volutpat odio facilisis. Odio eu feugiat pretium nibh.
            Mauris vitae ultricies leo integer malesuada. Blandit libero
            volutpat sed cras ornare arcu dui. Blandit massa enim nec dui nunc
            vulputate ut. Lectus quam id leo in vitae turpis massa sed
          </p>
          <a href="#" class="btn btn--green">Book Now</a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import CardBox from "./components/CardBox.vue";

export default {
  components: {
    CardBox,
  },
  data() {
    return {};
  },
};
</script>