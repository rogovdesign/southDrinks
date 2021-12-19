<template>
  <header class="header">
    <div class="container">
      <div class="header__container">
        <div class="header__left">
          <div class="header__logo-container">
            <router-link to="/"
              ><img src="@/img/logo.png" alt="" class="header__logo"
            /></router-link>
          </div>

          <nav>
            <ol class="header__nav">
              <li class="header__nav-item">
                <router-link
                  class="link"
                  to="/"
                  exact-active-class="link-active"
                  >О компании</router-link
                >
              </li>
              <li class="header__nav-item">
                <router-link
                  class="link"
                  to="/product"
                  exact-active-class="link-active"
                  >Продукция</router-link
                >
              </li>
              <li class="header__nav-item">
                <router-link
                  class="link"
                  to="/contacts"
                  exact-active-class="link-active"
                  >Контакты</router-link
                >
              </li>
            </ol>
          </nav>
        </div>

        <div class="header__right">
          <ol>
            <li class="header__nav-phone">
              <a class="link__phone" href="tel:88616265015"
                >8 (86162) 6-50-15</a
              >
            </li>
            <li class="header__nav-phone">
              <a class="link__phone" href="tel:+79182893779"
                >8 (918) 289-37-79</a
              >
            </li>
          </ol>
          <button class="header__button">Заказать звонок</button>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped lang="scss">

  .header-p {
    font-size: 18px;
    font-family: "Raleway";
  }
  body {
    background-color: #faf5e9;
  }

  .section {
    background-color: #faf5e9;
  }

  .container {
    display: block;
    margin: 0 100px;
  }

  .link {
    display: inline-block;
    padding: 10px 0;
    line-height: 1.3;
    color: #4b4961;

    background: no-repeat 0 100%;
    background-image: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
    background-size: 0% 4px;
    transition: background-size 0.8s ease;
    &:hover {
      color: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
      background-size: 100% 4px;
    }
  }

  .link__phone {
    color: #4b4961;
    transition: 0.3s;
    &:hover {
      
      color: black;
    }
  }

  .link__phone-active {
    color: #ffd25a;
  }

  .link-active {
    background: no-repeat 0 100%;
    background-image: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
    background-size: 100% 4px;
  }

  .header {
    background-color: #faf4e8;
  }
  .header__container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }

  .header__left {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    gap: 80px;
  }

  .header__right {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    gap: 80px;
  }

  .header__logo-container {
    background-color: white;
    border-radius: 0px 0px 10px 10px;
    box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.15);
  }

  .header__logo {
    width: 186px;
    margin: 18px 24px;
  }

  .header__nav {
    list-style: none;
  }

  .header__nav-item {
    font-weight: 400;
    font-size: 22px;
    display: inline; /* Отображать как строчный элемент */
    margin-right: 80px; /* Отступ слева */
  }

  .header__nav-phone {
    font-weight: 400;
    font-size: 22px;
    list-style: none;
    padding: 3px;
  }

  .header__button {
    font-family: "comfortaa";
    padding: 20px 43px;
    background: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
    border-radius: 10px;
    font-size: 20px;
    transition-duration: 0.5s;

    &:hover {
      box-shadow: 0px 0px 15px rgba(255, 210, 90, 0.6);
      background: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
    }

    &:active {
      box-shadow: 0px 0px 15px rgba(255, 210, 90, 0.4), inset 0px 4px 4px rgba(0, 0, 0, 0.1);
      transition-duration: 0s;
      background: linear-gradient(269.21deg, #ffd25a 0.49%, #ffc52b 100%);
    }
  }
</style>
