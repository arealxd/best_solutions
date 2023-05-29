<script setup lang="ts"></script>

<template>
  <div class="hero-bg">
    <div class="container hero-bg__content">
      <div class="hero-bg__content-blue__languages-mobile">
        <p>RU</p>
        <P>KZ</P>
      </div>
      <div class="hero-bg__content-text">
        <p>Онлайн кредит без справок и поручителей</p>
        <p>Сравним и подберем лучшие условия для Вас!</p>
      </div>
      <div class="hero-bg__content-blue">
        <div class="hero-bg__content-blue__languages">
          <p>RU</p>
          <P>KZ</P>
        </div>
        <div class="hero-bg__content-blue__phone">
          <img src="/img/mobileIcon.png" alt="" />
          <p>6901</p>
        </div>
        <p class="hero-bg__content-blue__call">звонок бесплатный</p>
        <div class="hero-bg__content-blue__number">
          <img src="/img/phone.png" alt="" />
          <p>8 708 808 6901</p>
        </div>
      </div>
    </div>
  </div>
  <div class="container cards">
    <div class="cards__column" v-for="i in 2" :key="i">
      <div class="cards__column-card" v-for="n in 3" :key="n">
        <img class="cards__column-card__bank" src="/img/bankLogo.png" alt="" />
        <div class="cards__column-card__hr"></div>
        <p class="cards__column-card__percent">Без переплат 0,1%</p>
        <div class="cards__column-card__hr"></div>
        <div class="cards__column-card__description">
          <div class="cards__column-card__description-texts">
            <p>Первый</p>
            <p>до 145 000 ₸</p>
          </div>
          <div class="cards__column-card__description-texts">
            <p>Сумма</p>
            <p>мах 145 000 ₸</p>
          </div>
          <div class="cards__column-card__description-texts">
            <p>Возраст</p>
            <p>19 до 70</p>
          </div>
          <div class="cards__column-card__description-texts">
            <p>Время получения</p>
            <p>15 мин.</p>
          </div>
        </div>
        <button class="cards__column-card__apply">Подать заявку</button>
      </div>
    </div>
    <div class="cards_instruction-column">
      <div class="cards_instruction-column__step">
        <p class="cards_instruction-column__step-text">1.</p>
        <p class="cards_instruction-column__step-text">
          Позвонив нам Вы получите подробную консультацию по всем Вашим вопросам от наших
          операторов.
        </p>
      </div>
      <div class="cards_instruction-column__hr"></div>
      <div class="cards_instruction-column__step">
        <p class="cards_instruction-column__step-text">2.</p>
        <p class="cards_instruction-column__step-text">
          Для получения займа достаточно одного документа - удостоверение личности. Без залога, без
          дохода, без пенсионных отчислений, с действующим кредитом, пенсионерам и студентам.
        </p>
      </div>
      <div class="cards_instruction-column__hr"></div>
      <div class="cards_instruction-column__step">
        <p class="cards_instruction-column__step-text">3.</p>
        <p class="cards_instruction-column__step-text">
          Режим работы нашего колл-центра 6901 с 09:00 - 20:00 ежедневно без выходных.
        </p>
      </div>
      <div class="cards_instruction-column__hr"></div>
      <div class="cards_instruction-column__step">
        <p class="cards_instruction-column__step-text">4.</p>
        <p class="cards_instruction-column__step-text">
          Наши операторы помогут Вам оформить заявку правильно, для повышения вероятности одобрения.
        </p>
      </div>
      <div class="cards_instruction-column__hr"></div>
      <div class="cards_instruction-column__step">
        <p class="cards_instruction-column__step-text">5.</p>
        <p class="cards_instruction-column__step-text">
          Если Вы зашли на сайт в нерабочее время нашего центра 6901, то Вы можете попробовать
          самостоятельно оформить займ выбрав одно из представленных МФО кликнув на “Подать заявку”,
          пошагово заполнив поля. Наши операторы помогут Вам оформить заявку правильно и быстро.
        </p>
      </div>
    </div>
  </div>
  <div class="container footer">
    <div class="footer__hr"></div>
    <div class="footer__text">Данный сайт предоставляет исключительно информационные услуги!</div>
    <div class="footer__hr"></div>
    <div class="footer__copyright">© 2017 - 2023 Best Solutions</div>
  </div>
</template>

<style scoped lang="scss">
.hero-bg {
  background-image: url('/img/heroBg.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 500px;
  width: 100%;
}
.hero-bg__content {
  display: flex;
  justify-content: space-between;
  height: 100%;
  .hero-bg__content-text {
    display: flex;
    flex-direction: column;
    gap: 15px;
    :nth-child(1) {
      font-weight: 700;
      font-size: 48px;
      color: #ffffff;
      width: 650px;
      line-height: normal;
      text-transform: uppercase;
      margin-top: 247px;
    }
    :nth-child(2) {
      font-weight: 400;
      font-size: 20px;
      color: #ffffff;
    }
  }
  .hero-bg__content-blue {
    display: flex;
    flex-direction: column;
    padding: 46px 26px 86px 26px;
    background: #3a1bb5;
    .hero-bg__content-blue__languages {
      display: flex;
      align-items: center;
      gap: 10px;
      margin: 0 auto;
      :nth-child(1) {
        font-weight: 700;
        font-size: 28px;
        text-transform: uppercase;
        color: #feb119;
        border: 2px solid #feb119;
        border-radius: 6px;
        padding: 0 5px;
        line-height: 1.2;
      }
      :nth-child(2) {
        font-weight: 700;
        font-size: 28px;
        text-transform: uppercase;
        color: #ffffff;
      }
    }
    .hero-bg__content-blue__phone {
      margin-top: 88px;
      display: flex;
      align-items: center;
      gap: 20px;
      border: 5px solid #feb119;
      border-radius: 20px;
      justify-content: center;
      padding: 14px 0;
      :nth-child(2) {
        margin-top: -10px;
        font-weight: 700;
        font-size: 80px;
        display: flex;
        align-items: center;
        text-align: center;
        color: #feb119;
        line-height: 94px;
      }
    }
    .hero-bg__content-blue__call {
      font-weight: 700;
      font-size: 28px;
      line-height: 48px;
      text-transform: uppercase;
      color: #ffffff;
      margin-top: 10px;
    }
    .hero-bg__content-blue__number {
      display: flex;
      align-items: center;
      gap: 20px;
      margin-top: 20px;
      :nth-child(2) {
        font-weight: 500;
        font-size: 36px;
        line-height: 42px;
        display: flex;
        align-items: center;
        text-align: center;
        letter-spacing: 0.03em;
        color: #ffffff;
      }
    }
  }
}
.cards {
  display: flex;
  margin-top: 60px;
  justify-content: space-between;
  padding-bottom: 60px;
  gap: 40px;
  .cards__column {
    display: flex;
    flex-direction: column;
    gap: 40px;
    width: 100%;
    max-width: 360px;
    .cards__column-card {
      padding: 22px 30px 30px 30px;
      background: #f8f8f8;
      border: 1px solid rgba(0, 0, 0, 0.15);
      border-radius: 6px;
      display: flex;
      flex-direction: column;
      align-items: center;
      transition: all 0.3s ease;
      .cards__column-card__bank {
        margin-bottom: 22px;
      }
      .cards__column-card__hr {
        width: 100%;
        border: 1px solid rgba(0, 0, 0, 0.15);
      }
      .cards__column-card__percent {
        font-weight: 500;
        font-size: 18px;
        line-height: 21px;
        display: flex;
        align-items: center;
        text-align: center;
        color: #000000;
        margin: 16px 0;
      }
      .cards__column-card__description {
        display: flex;
        flex-direction: column;
        margin-top: 33px;
        gap: 20px;
        width: 100%;
        .cards__column-card__description-texts {
          display: flex;
          align-items: center;
          justify-content: space-between;
          p {
            font-weight: 400;
            font-size: 14px;
            line-height: 16px;
            color: #000000;
            padding: 0;
            margin: 0;
          }
        }
      }
      .cards__column-card__apply {
        padding: 18px 0px;
        width: 100%;
        margin-top: 48px;
        background: #66d144;
        border-radius: 6px;
        font-weight: 700;
        font-size: 14px;
        line-height: 16px;
        text-align: center;
        color: #ffffff;
        transition: all 0.3s ease;
      }
      .cards__column-card__apply:hover {
        background: #53b135;
      }
    }
    .cards__column-card:hover {
      border: 1px solid #66d144;
    }
  }
  .cards_instruction-column {
    display: flex;
    flex-direction: column;
    padding: 29px 25px 29px 25px;
    background: rgba(255, 138, 1, 0.05);
    width: 100%;
    max-width: 360px;
    .cards_instruction-column__step {
      display: flex;
      align-items: flex-start;
      gap: 10px;
      &-text {
        font-weight: 400;
        font-size: 22px;
        line-height: 36px;
        color: #000000;
      }
    }
    &__hr {
      width: 100%;
      border: 1px solid #ff8a01;
      margin: 20px 0;
    }
  }
}
.footer {
  display: flex;
  flex-direction: column;
  align-items: center;
  &__hr {
    width: 100%;
    border: 1px solid rgba(0, 0, 0, 0.15);
  }
  &__text {
    font-weight: 500;
    font-size: 20px;
    line-height: 32px;
    text-align: center;
    color: #000000;
    margin: 20px 0;
  }
  &__copyright {
    font-weight: 400;
    font-size: 14px;
    line-height: 24px;
    text-align: center;
    color: #000000;
    padding: 10px 0;
  }
}

@media screen and (max-width: 520px) {
  .hero-bg {
    height: 730px;
  }
  .hero-bg__content {
    display: flex;
    flex-direction: column;
    .hero-bg__content-blue__languages-mobile {
      display: flex;
      align-items: center;
      gap: 10px;
      margin: 0 auto;
      background: #3a1bb5;
      padding: 13px 16px;
      position: absolute;
      right: 0;
      top: 0;
      :nth-child(1) {
        font-weight: 700;
        font-size: 22px;
        text-transform: uppercase;
        color: #feb119;
        border: 2px solid #feb119;
        border-radius: 6px;
        padding: 0 5px;
        line-height: 1.2;
      }
      :nth-child(2) {
        font-weight: 700;
        font-size: 22px;
        text-transform: uppercase;
        color: #ffffff;
      }
    }

    .hero-bg__content-blue {
      .hero-bg__content-blue__languages {
        display: none;
      }
    }
    .hero-bg__content-text {
      display: flex;
      flex-direction: column;
      gap: 10px;
      padding-left: 40px;
      margin-bottom: 20px;
      :nth-child(1) {
        font-weight: 700;
        font-size: 24px;
        color: #ffffff;
        width: 250px;
        line-height: normal;
        text-transform: uppercase;
        margin-top: 190px;
      }
      :nth-child(2) {
        font-weight: 400;
        font-size: 18px;
        color: #ffffff;
        width: 250px;
      }
    }
  }
  .hero-bg__content .hero-bg__content-blue .hero-bg__content-blue__phone {
    margin-top: 0;
    :nth-child(2) {
      font-size: 64px;
    }
  }
  .hero-bg__content .hero-bg__content-blue {
    padding: 30px 70px 28px 40px;
    margin-bottom: 52px;
  }
  .hero-bg__content .hero-bg__content-blue .hero-bg__content-blue__call {
    font-size: 22px;
  }
  .hero-bg__content .hero-bg__content-blue .hero-bg__content-blue__number :nth-child(2) {
    font-size: 28px;
  }
  .cards .cards_instruction-column .cards_instruction-column__step-text {
    font-size: 18px;
  }
  .cards {
    flex-direction: column-reverse;
    margin-top: 40px;
    padding: 0 20px;
    .cards__column {
      max-width: 100%;
    }
    .cards_instruction-column {
      max-width: 100%;
    }
  }
  .footer {
    padding: 0 20px;
    margin-top: 50px;
    &__hr {
      width: 100%;
      border: 1px solid rgba(0, 0, 0, 0.15);
    }
    &__text {
      font-weight: 500;
      font-size: 16px;
      line-height: 24px;
      text-align: center;
      color: #000000;
      margin: 20px 0;
    }
    &__copyright {
      font-weight: 400;
      font-size: 12px;
      line-height: 24px;
      text-align: center;
      color: #000000;
      padding: 10px 0;
    }
  }
}
</style>
