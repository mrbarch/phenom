<template>
  <div>
    <div class="join">
      <div class="container">
        <div class="join__main">
          <div class="join__main-1">
            <img src="/alert-symbol.png" alt="alert" class="join__main-alert">
            <h1 class="join__main-title">Email verification</h1>
            <p class="join__main-subtitle">
              Please go to your email account to find a link <br> for your account activation.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.join {
  background-image: url('/background-header.png');
  background-size: 100%;
  background-repeat: no-repeat;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
  height: 81rem;

  &__main {
    height: 64rem;

    &-alert {
      position: relative;
      left: 56.7rem;
      top: 31rem;
    }

    &-title {
      font-family: Raleway-Bold, sans-serif;
      width: 100%;
      font-style: normal;
      font-weight: bold;
      font-size: 3rem;
      line-height: 3.5rem;
      text-align: center;
      color: #FFFFFF;
      padding-top: 33rem;
      margin: 0;
    }

    &-subtitle {
      font-family: Raleway-Medium, sans-serif;
      font-style: normal;
      font-weight: 500;
      font-size: 1.2rem;
      line-height: 2.3rem;
      text-align: center;
      letter-spacing: 0.01em;
      color: #CED4DA;
      margin: 0;
      padding-top: 1.6rem;
    }
  }

  &__title {
    padding-top: 9rem;
    font-weight: 700;
    text-align: center;
    font-style: normal;
    font-size: 5rem;
    line-height: 5.1rem;
    color: white;
    margin-bottom: 0;
    letter-spacing: 0.1rem;
  }

  &__subtitle {
    text-align: center;
    color: white;
    font-size: 1.2rem;
    padding-top: 2.3rem;
    width: 29rem;
    margin: auto;
    line-height: 1.9rem;
    letter-spacing: -0.04rem;
  }

  &__block {
    padding-top: 5.4rem;

    &-login {
      position: relative;
      left: 15rem;
      top: 3rem;
      font-style: normal;
      font-weight: 500;
      font-size: 1rem;
      line-height: 1rem;
      letter-spacing: 0.02rem;
      color: #8898AA;

      span {
        color: blue;
      }
    }

    &-privacy {
      display: flex;
      align-items: flex-end;
      grid-auto-rows: 30rem;
      justify-content: space-between;
      width: 19.5rem;
      padding-top: 1rem;

      &-text {
        color: #8898AA;
        margin: 0;
        align-self: center;
        padding: 1rem 0;
        width: 17rem;

        span {
          color: #0F38E2;
        }
      }

      &-checkbox[type=checkbox] {
        background: #FFFFFF !important;
        border: 1px solid #CBD3DD !important;
        height: 1.6rem !important;
        width: 1.6rem !important;
        margin: 0;
        align-self: center;
        border-radius: 50% !important;

      }
    }

    &-input {
      height: 3.2rem;
      width: 21.3rem;
      background: #FFFFFF;
      border: 1px solid #CBD3DD;
      border-radius: 6px;
      outline: 0;
      outline-offset: 0;
    }

    &-bg {
      width: 45.8rem;
      height: 25.2rem;
      background-color: #fff;
      margin: auto;
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-column-gap: 2.5rem;
      grid-auto-rows: 3.5rem;
      grid-row-gap: 1.2rem;
      padding: 5rem 6rem 5rem 6rem;
    }

    &-btn {
      margin-top: 0.23rem;
      background: #0F38E2;
      box-shadow: 0 1px 3px rgba(0, 0, 0, 0.08), 0 4px 6px rgba(50, 50, 93, 0.1);
      border-radius: 56px;
      height: 4rem;
      color: white;
      letter-spacing: .07rem;
      border: none;
    }

    &-check {
      text-align: right;
      color: #8898AA;
      margin-top: -.05rem;
      letter-spacing: -0.06rem;

      span {
        color: green;
      }
    }

    &-first {
      background: url(/person.png) no-repeat 1rem;
      padding-left: 3rem;
      width: 18.5rem;
    }

    &-placeholder::placeholder {
      padding-right: 2.6rem;
      letter-spacing: 0.03rem;
      color: #ADB5BD;
      font-family: Raleway-Medium, sans-serif;
      font-style: normal;
    }

    &-last {
      background: url(/person.png) no-repeat 1rem;
      padding-left: 3rem;
      width: 18.5rem;
    }

    &-email {
      background: url(/email.png) no-repeat .5rem;
      padding-left: 3rem;
      width: 18.5rem;
    }

    &-country {
      background: url(/earth.png) no-repeat 1rem, url(/arrow-country.png) no-repeat 19.8rem;
      padding-left: 3rem;
      width: 18.5rem;
    }

    &-password {
      background: url(/lock.png) no-repeat 1rem, url(/eye.png) no-repeat 19.8rem;
      padding-left: 3rem;
      width: 18.5rem;
    }

    &-repeat {
      background: url(/lock.png) no-repeat 1rem, url(/eye.png) no-repeat 19.8rem;
      padding-left: 3rem;
      width: 18.5rem;
    }

    &-referral {
      background: url(/rocket.png) no-repeat 1rem;
      padding-left: 3rem;
      width: 18.5rem;
    }
  }

  &__footer {
    display: flex;
    padding-top: 10.5rem;
    width: 100%;
    justify-content: space-between;
    opacity: 0.4;

    &-left {
      color: white;
      width: 11rem;
      letter-spacing: 0.043rem;
      padding-left: 0.3rem;
    }

    &-center {
      color: white;
      width: 55.5rem;
      display: flex;
      justify-content: space-between;
      padding-left: 0;
      padding-right: 1.2rem;
    }

    &-right {
      display: flex;
      justify-content: space-between;
      width: 10.5rem;

      :nth-child(1) {
        width: 2rem;
        height: 2rem;
        padding-top: .5rem;
      }

      :nth-child(2) {
        width: 2rem;
        height: 2rem;
        padding-top: .5rem;
        padding-right: -.2rem;
      }

      :nth-child(3) {
        width: 2rem;
        height: 2rem;
        padding-top: .5rem;
        padding-right: .8rem;
      }
    }
  }
}
</style>
