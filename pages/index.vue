<template>
  <div>
    <div class="join">
      <div class="container">
        <h1 class="join__title">
          Join now
        </h1>
        <div class="join__subtitle">
          Use these awesome forms to login or create new
          account in your project for free.
        </div>
        <div class="join__block">
          <div class="join__block-bg">
            <input placeholder="First name"
                   type="text"
                   class="join__block-first join__block-input join__block-placeholder">
            <input placeholder="Last name"
                   type="text"
                   class="join__block-last join__block-input join__block-placeholder">
            <input placeholder="Email"
                   type="text"
                   class="join__block-email join__block-input join__block-placeholder">
            <div class="dropdown">
              <input @click="toggleShow" placeholder="Country"
                     class="join__block-country join__block-input join__block-placeholder">
              <ul id="myDropdown" class="dropdown-content">
                <li class="join__block-placeholder">Ukraine</li>
                <li class="join__block-placeholder">England</li>
                <li class="join__block-placeholder">Romania</li>
              </ul>
            </div>
            <input placeholder="Password"
                   type="text"
                   class="join__block-password join__block-input join__block-placeholder">
            <input placeholder="Repeat password"
                   type="text"
                   class="join__block-repeat join__block-input join__block-placeholder">
            <input placeholder="Referral ID"
                   type="text"
                   class="join__block-referral join__block-input join__block-placeholder">
            <div class="join__block-check">Password strength: <span>strong</span></div>
            <div class="join__block-privacy">
              <input type="checkbox" class="join__block-privacy-checkbox">
              <p class="join__block-privacy-text">I agree with the <span>Privacy Policy</span></p>
            </div>
            <button class="join__block-btn">Create account</button>
            <div class="join__block-login">Already have an account? <span>Log in</span></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    toggleShow() {
      document.getElementById("myDropdown").classList.toggle("show");
    }
  }
}
</script>

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
      font-weight: 100;
      height: 3.5rem;
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
  .dropbtn {
    background-color: #3498DB;
    color: white;
    padding: 16px;
    font-size: 16px;
    border: none;
    cursor: pointer;
  }

  .dropbtn:hover, .dropbtn:focus {
    background-color: #2980B9;
  }

  .dropdown {
    position: relative;
    display: inline-block;
  }

  .dropdown-content {
    width: 19rem;
    border-radius: 0.5rem;
    display: none;
    position: absolute;
    background-color: white;
    min-width: 160px;
    overflow: auto;
    box-shadow: 0 8px 16px 0 rgb(0 0 0 / 20%);
    z-index: 1;
  }

  .dropdown-content li {
    color: #CBD3DD;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
  }

  .dropdown li:hover {
    background-color: #ddd;
  }

  .show {
    display: block;
  }
}
</style>
