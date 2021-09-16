<template>
  <div>
    <header>
      <div class="container">
        <div class="header">
          <div class="header__left">
            <img src="/logo.png" alt="logo" class="header__logo">
            <div class="header__lang">
              <img src="/lang-usa.png" alt="usa" class="header__lang-img">
              <p class="header__lang-text">English</p>
              <img src="/arrow-lang.png" alt="arrow" class="header__lang-arrow">
            </div>
          </div>
          <div class="header__right">
            <div class="header__menu">
              <button class="header__menu-log">Log in</button>
              <button class="header__menu-join">Join now</button>
            </div>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<style lang="scss">

.header__left {
  display: flex;
  justify-content: space-between;
  width: 22.3rem;
  height: 2rem;
}
.header__right {
  display: flex;
  justify-content: space-between;
  width: 18.5rem;
  padding-right: .8rem;
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 8rem;
  &__logo {
    width: 8rem;
    height: 2.5rem;
  }
}
.header__lang {
  font-family: Raleway-Medium, sans-serif;
  display: flex;
  width: 6rem;
  justify-content: space-between;
  align-items: center;
  height: 2rem;
  padding-bottom: .9rem;
  font-weight: 500;
  font-size: 1rem;
  line-height: 1rem;
  &-text {
    color: white;
  }
  &-img{
    height: 1rem;
    width: 1rem;
  }
  &-arrow {
    height: .6rem;
    width: .5rem;
  }
}
.header__menu {
  display: flex;
  justify-content: space-between;
  width: 23rem;
  padding-bottom: 1rem;

  &-log {
    font-style: normal;
    font-weight: bold;
    font-size: 1rem;
    line-height: 1rem;
    border: 1px solid #FFFFFF;
    box-sizing: border-box;
    border-radius: 60px;
    background-color: transparent;
    height: 43px;
    width: 98px;
    color: white;
  }
  &-join {
    font-style: normal;
    font-weight: bold;
    font-size: 1rem;
    line-height: 1rem;
    color: white;
    background: #24203F;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.08), 0px 4px 6px rgba(50, 50, 93, 0.1);
    border-radius: 60px;
    height: 43px;
    width: 131px;
    border: none;
    letter-spacing: 0.03rem;
  }
}
</style>
