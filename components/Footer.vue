<template>
  <div>
    <footer>
        <div class="container">
          <div class="footer">
          <div class="footer__left">
            <p class="footer__left-text">© 2020 TC GROUP</p>
          </div>
          <ul class="footer__center">
            <li class="footer__center-text">Company info</li>
            <li class="footer__center-text">Terms and conditions</li>
            <li class="footer__center-text">Memorandum of association</li>
            <li class="footer__center-text">Privacy policy</li>
            <li class="footer__center-text">AML Policy</li>
          </ul>
          <div class="footer__right">
            <img src="/telegram.png" alt="telegram" class="footer__right-img">
            <img src="/instagram.png" alt="instagram" class="footer__right-img">
            <img src="/facebook.png" alt="facebook" class="footer__right-img">
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss">
.footer {
  position: relative;
  top: 56.3rem;
  display: flex;
  padding-top: 10.5rem;
  width: 100%;
  justify-content: space-between;
  opacity: 0.4;

  &__left {
    color: white;
    width: 11rem;
    letter-spacing: 0.043rem;
    padding-left: 0.3rem;
  }

  &__center {
    color: white;
    width: 55.5rem;
    display: flex;
    justify-content: space-between;
    padding-left: 0;
    padding-right: 1.2rem;
  }

  &__right {
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


</style>
