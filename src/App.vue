<template>
  <div class="container">
    <section class="form">
      <a href="./sign-up.html" class="form-logo logo">Your Logo</a>
      <div class="form-content">
        <h1 class="form-title">Sign in</h1>
        <p class="form-subtitle">If you don’t have an account register</p>
        <p class="form-subtitle">
          You can <a href="#" class="form-link">Register here !</a>
        </p>
        <form action="#" class="form-form-box form-box">
          <div class="form-box-input-box input-box">
            <label class="input-box-info" for="email">Email</label>
            <label class="input-box-icon" for="email"
              ><img src="img/email.svg" alt="email"
            /></label>
            <input
              type="email"
              name="email"
              id="email"
              placeholder="Enter your email address"
            />
          </div>
          <div class="form-box-input-box input-box">
            <label class="input-box-info" for="password">Password</label>
            <label class="input-box-icon" for="password"
              ><img src="img/password.svg" alt="password"
            /></label>
            <input
              type="password"
              name="password"
              id="password"
              placeholder="Enter your password"
            />
          </div>
          <div class="form-box-btn-box btn-box">
            <button type="submit">Login</button>
          </div>
          <div class="form-box-social">
            <span class="form-box-social-info">or continue with</span>
            <div class="form-box-social-items">
              <a href="#"><img src="img/facebook.svg" alt="facebook" /></a>
              <a href="#"><img src="img/apple.svg" alt="apple" /></a>
              <a href="#"><img src="img/google.svg" alt="google" /></a>
            </div>
          </div>
        </form>
      </div>
    </section>
    <section class="promo">
      <div class="promo-box">
        <div class="promo-content">
          <img src="img/saly.png" alt="saly" class="promo-img" />
          <h1 class="promo-title">Sign in to name</h1>
          <p class="promo-subtitle">Lorem Ipsum is simply</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

*,
*::after,
*::before {
  box-sizing: inherit;
}

body {
  width: 100%;
  font-family: "Poppins", sans-serif;
  font-size: 16px;
  min-height: 100vh;
}

.container {
  width: 100%;
  display: flex;
}

.logo {
  font-weight: 600;
  font-size: 20px;
  line-height: 30px;
  color: #000000;
  text-decoration: none;
}

.form {
  flex: 1 0 auto;
  flex-direction: column;
  margin-top: 31px;
  margin-left: 42px;
}
@media (max-width: 1200px) {
  .promo {
    padding: 0 20px;
  }
}

.form-content {
  width: 100%;
  max-width: 431px;
  padding-top: 102px;
  padding-bottom: 102px;
  align-items: center;
  /* не работает из-за auto*/
}

.form-title {
  font-weight: 500;
  font-size: 30px;
  line-height: 45px;
  color: #000000;
  display: block;
  margin-bottom: 22px;
}

.form-subtitle {
  font-size: 16px;
  line-height: 24px;
  color: #000000;
  margin-bottom: 6px;
}

.form-link {
  color: #0c21c1;
  font-weight: 600;
  font-size: 16px;
  line-height: 24px;
  text-decoration: none;
  margin-bottom: 55px;
}

.input-box {
  box-sizing: border-box;
  margin-bottom: 49px;
  width: 100%;
  padding-bottom: 9px;
  padding-left: 27px;
  border-bottom: 2px solid #999999;
}

.input-box:hover {
  border-bottom: 2px solid #000842;
  color: #000842;
}

.input-box-info {
  display: block;
  margin-bottom: 11px;
  font-weight: 500;
  font-size: 13px;
  line-height: 20px;
  color: #999999;
  user-select: none;
}

.form-box {
  margin-top: 55px;
}

.input-box-icon {
  margin-bottom: 0px;
}

.btn-box button {
  margin-top: 109px;
  background: #0c21c1;
  box-shadow: 0px 4px 26px rgba(0, 0, 0, 0.25);
  border-radius: 32px;
  font-weight: 500;
  font-size: 17px;
  line-height: 26px;
  color: #ffffff;
  width: 100%;
  text-align: center;
  cursor: pointer;
  padding-top: 14px;
  padding-bottom: 14px;
}

.form-box-social {
  margin-top: 36px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.form-box-social-info {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #b5b5b5;
  margin-bottom: 31px;
}

.form-box-social-items {
  display: flex;
}

.form-box-social-items a {
  margin-right: 20px;
}

.promo {
  flex: 0 0 735px;
  display: flex;
  flex-direction: column;
  padding: 21px;
}

.promo-box {
  flex-grow: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #000842;
  border-radius: 15px;
}

.promo-content img {
  width: 100%;
  max-width: 559px;
  height: auto;
  margin-bottom: 90px;
}

.promo-content h1 {
  font-weight: 600;
  font-size: 40px;
  line-height: 60px;
  color: #ffffff;
  margin-bottom: 4px;
}

.promo-subtitle {
  font-weight: 300;
  font-size: 20px;
  line-height: 30px;
  color: #ffffff;
  display: block;
}

@media (max-width: 1200px) {
  .promo {
    display: none;
  }
}
</style>
