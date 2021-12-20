<template>
  <footer class="footer">
    <div class="footer__up">
      <div class="container footer__container">
        <div class="footer__form-text">
          <h3 class="h3">Ждем ваших заказов</h3>
          <p class="footer__text">
            Чтобы стать нашим клиентом, свяжитесь по телефону с нашими
            менеджерами либо оставьте заявку на сайте. ООО «Кубань Агро-продукт»
            – ваш надежный производитель и поставщик натуральных соков и
            напитков.
          </p>
        </div>

        <div class="footer__form">
          <form action="post">
            <div class="form__align">
              <div class="form__align-row">
                <input
                  type="text"
                  placeholder="Ваше имя"
                  class="input input__up"
                />
                <input
                  type="text"
                  placeholder="Номер телефона"
                  class="input input__up"
                />
              </div>

              <input
                type="text"
                placeholder="Комментарий"
                class="input input__down"
              />

              <div class="form__checkbox-align">
                <input type="checkbox" v-model="toggle" />
                <p>
                  Даю согласие на обработку персональных данных и подтверждаю
                  свое ознакомление с
                  <a href="" class="link link__orange"
                    >политикой обработки персональных данных</a
                  >
                  компании
                </p>
              </div>

              <button class="button footer__button">Отправить</button>
            </div>
          </form>
        </div>
      </div>
    </div>

    <div class="main__footer">
      <div class="container main__footer-container">
        <div class="main__footer-left">
          <router-link to="/"
            ><img src="@/img/logo.png" alt="" class="footer__logo"
          /></router-link>

          <nav>
            <ol class="footer__nav">
              <li class="footer__nav-item">
                <router-link class="link" to="/">О компании ></router-link>
              </li>
              <li class="footer__nav-item">
                <router-link class="link" to="/product"
                  >Продукция ></router-link
                >
              </li>
              <li class="footer__nav-item">
                <router-link class="link" to="/contacts"
                  >Контакты ></router-link
                >
              </li>
            </ol>
          </nav>

          <div class="footer__item1">
            <p class="h4">Юр. Адрес</p>
            <p class="p">
              Краснодарский край,<br />
              г. Геленджик, ул. Кирова, 117
            </p>
            <a href="" class="link">klohkonikita@mail.ru</a>
          </div>

          <div class="footer__item1">
            <p class="h4">Производство</p>
            <p class="p">
              Краснодарский край, Динской р-н,<br />
              ст. Динская, ул. Краснодарская, 15 а.
            </p>
            <a href="" class="link">ooo_kap@mail.ru</a>
          </div>
        </div>
        <div class="main__footer-right">
          <ol>
            <li class="footer__nav-phone">
              <a class="link__phone" href="tel:88616265015"
                >8 (86162) 6-50-15</a
              >
            </li>
            <li class="footer__nav-phone">
              <a class="link__phone" href="tel:+79182893779"
                >8 (918) 289-37-79</a
              >
            </li>
          </ol>
        </div>
      </div>
    </div>

    <div class="main__footer-down">
      <div class="footer__down-container">
        <p class="footer__policy">© napitki-uga.ru, 2021</p>
        <a href="" class="footer__policy">Политика конфиденциальности</a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped  lang="scss">


.container {
  display: block;
  margin: 0 100px;
}
.footer__container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 30px;
}

.footer__up {
  background-color: #fffcf3;
}

.h3 {
  font-family: Montserrat Alternates;
  font-weight: bold;
  font-size: 48px;
  line-height: 60px;
  color: #4b4961;
  margin-bottom: 20px;
  margin-top: 70px;
}

.footer__text {
  font-family: Raleway;
  font-size: 24px;
  line-height: 150%;
  color: #a1a1a1;
}

.footer__form-text {
  flex-basis: 50%;
}

.footer__form {
  margin-top: 70px;
  flex-basis: 50%;
}

.form__align {
  display: flex;
  flex-direction: column;
  gap: 30px;
}

.form__align-row {
  display: flex;
  flex-direction: row;
  gap: 30px;
  justify-content: space-between;
}

.input__up {
  width: 100%;
}

.input {
  padding: 20px;
  background: rgba(255, 255, 255, 0.4);
  border: 1px solid #dfdfdf;
  box-sizing: border-box;
  border-radius: 10px;
  font-family: raleway;
  font-size: 24px;
  line-height: 28px;

  color: #636363;
}
.input::placeholder {
  font-family: raleway;
  font-size: 24px;
  line-height: 28px;

  color: #d0cec4;
}

.form__checkbox-align {
  display: flex;
  gap: 15px;
}

.link__orange {
  color: #ffd25a;
  text-decoration-line: underline;
}

.button {
  font-family: "comfortaa";
  padding: 20px 43px;
  background: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
  border-radius: 10px;
  font-size: 20px;
  transition-duration: 0.5s;
  margin-bottom: 75px;

  &:hover {
    box-shadow: 0px 0px 15px rgba(255, 210, 90, 0.6);
    background: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
  }

  &:active {
    box-shadow: 0px 0px 15px rgba(255, 210, 90, 0.4),
      inset 0px 4px 4px rgba(0, 0, 0, 0.1);
    transition-duration: 0s;
    background: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
  }
}

.main__footer {
  background-color: #faf5e9;
}
.main__footer-container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  padding: 30px 0;
}
.main__footer-left {
  display: flex;
  align-items: center;
  flex-direction: row;
  gap: 100px;
}

.main__footer-right {
  display: flex;
  flex-direction: row;
  gap: 100px;
}

.footer__logo {
  width: 186px;
}
.footer__nav {
  list-style: none;
}

.footer__nav-item {
  font-weight: 400;
  padding: 7px 0;
  font-size: 18px;
}

.link {
  color: #6a6a6a;
  transition: 0.3s ease;
  &:hover {
    color: #000000;
    text-decoration-line: underline;
  }
}

.footer__nav-phone {
  font-weight: 400;
  font-size: 22px;
  list-style: none;
  padding: 3px;
}

.link__phone {
  color: #4b4961;
  transition: 0.3s;
  &:hover {
    color: black;
  }
}

.h4 {
  font-weight: bold;
  font-size: 18px;
  margin-bottom: 15px;
  color: #4b4961;
}

.p {
  font-size: 18px;
  line-height: 22px;
  color: #6a6a6a;
}

.main__footer-down {
  background-color: #ece2ca;
}
.footer__down-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;

  padding: 20px 100px;
}

.footer__policy {
  color: #a9a9a9;
}
</style>
