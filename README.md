<style>
.header {
  /* цвета */
  --clr-ntrl-ltr: #ffffff;
  --clr-ntrl-lt: #f2f2f2;
  --clr-ntrl-dk: #1f1f1f;
  --clr-ntrl-dkr: #000000;
  --clr-brand-1: #2f80ed;

  /* размеры шрифта */
  --fs-xxxl: 120px;
  --fs-xxl: 102px;
  --fs-xl: 60px;
  --fs-l: 36px;
  --fs-m: 24px;
  --fs-s: 18px;

  /* уровни */
  --foreground: 5;
  --middle: 3;
  --background: 1;

  --pad-top-header: 30px;
  --pad-right-header: 0;
  --pad-bottom-header: 30px;
  --pad-left-header: 64px;
}

.header {
  position: relative;
  display: flex;
  flex-direction: row;
  align-items: center;
  height: 100vh;
  min-height: 600px;
  max-height: 756px;
  padding: var(--pad-top-header) var(--pad-right-header) var(--pad-bottom-header) var(--pad-left-header);
  background-color: var(--clr-ntrl-lt);
  box-sizing: border-box;
}

.header__logo {
  position: absolute;
  top: var(--pad-top-header);
  left: var(--pad-left-header);
  z-index: var(--foreground);
}

.header__title {
  margin: 0;
  width: 730px;
  line-height: 96px;
  color: var(--clr-ntrl-dkr);
  font-size: var(--fs-xxl);
  font-weight: 600;
  z-index: var(--middle);
}

.header__subtitle {
  position: absolute;
  left: var(--pad-left-header);
  bottom: var(--pad-bottom-header);
  margin: 0;
  width: 388px;
  color: var(--clr-ntrl-dkr);
  line-height: 25px;
  font-size: var(--fs-s);
  z-index: var(--middle);
}

.header__link {
  color: var(--clr-brand-1);
}

.header__main-illustration {
  position: absolute;
  right: 0;
  bottom: 0;
  width: 765px;
  height: 608px;
  z-index: var(--background);
}

.header__square-pic {
  position: absolute;
  top: 64px;
  right: 0;
  height: 568px;
  width: 568px;
  background-color: var(--clr-brand-1);
  z-index: var(--background);
}

</style>

<header class="header">
  <img class="logo header__logo" src="./images/logo_place_header.svg" alt='Логитип "Яндекс Практикум"'/>
  <h1 class="header__title">Научиться учиться</h1>
  <p class="header__subtitle">Какие современные и эффективные подходы к обучению вы можете использовать в своей жизни? <a class="header__link">Склонируйте репозиторий и узнайте!</a></p>
  <div class="header__square-pic"></div>
  <img class="header__main-illustration" src="./images/header-image.png" alt='Вырезка из картины "Опять двойка" Фёдора Решетникова'/>
</header>
