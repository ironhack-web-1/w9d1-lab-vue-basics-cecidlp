<template>
  <form>
    <h2>This is my form:</h2>
    <input type="text" class="login__input" placeholder="Name" /><br />
    <input type="email" class="login__input" placeholder="Email" />
    <button class="button login__submit">
      <span class="button__text">Log In Now</span>
      <i class="button__icon fas fa-chevron-right"></i>
    </button>
  </form>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Raleway:400,700");

form {
  font-family: Raleway;
  padding: 2% 2%;
  background: linear-gradient(
    to right,
    rgba(232, 204, 197, 1) 0%,
    rgba(232, 204, 197, 0.94) 42%,
    rgba(251, 240, 238, 0.86) 100%
  );
  color: #a62121;
  box-shadow: 17px 20px 22px -14px rgba(128, 128, 128, 0.4);
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding-bottom: 20px;
  width: 20%;
  border-radius: 10%;
}

.login__input {
  border: none;
  border-bottom: 2px solid #d1d1d4;
  background: none;
  padding: 10px;
  padding-left: 24px;
  font-weight: 700;
  width: 75%;
}

::placeholder {
  color: #a62121;
}

.login__submit {
  background: #fff;
  font-size: 14px;
  margin-top: 10%;
  margin-bottom: 10%;
  padding: 16px 20px;
  border-radius: 26px;
  border: 1px solid #d4d3e8;
  text-transform: uppercase;
  font-weight: 700;
  display: flex;
  align-items: center;
  width: 85%;
  color: #a62121;
  box-shadow: 0px 2px 2px #a62121;
  cursor: pointer;
  transition: 0.2s;
}
</style>
