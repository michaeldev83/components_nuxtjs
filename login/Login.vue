<template>
  <section class="main_login">
    <div class="login">
      <h2>Connexion</h2>
      <div class="items">
        <label for="email"></label>
        <input type="email" name="email" id="email" placeholder="Email" autocomplete="true">
      </div>
      <div class="items">
        <label for="password"></label>
        <input type="password" name="password" id="password" placeholder="Password">
      </div>
      <button class="btn" type="submit">Connexion</button>
      <nuxt-link to="/">Créer un compte.</nuxt-link>
    </div>
  </section>
</template>

<style scoped>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.main_login {
  box-sizing: border-box;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Arial, Helvetica, sans-serif;
  padding: 10px;
  background-color: rgba(60, 159, 240);
  
}
.main_login .login {
  width:400px;
  min-width: 280px;
  margin: 0 auto;
  border-radius: 10px;
  padding: 40px 20px;
  color: rgb(100,100,100);
  background-color: #fff;
  box-shadow: 0 0 15px 2px rgba(0,0,0,0.3);
}
.login h2 {
  text-align: center;
  padding: 0 0 30px;
}
.items {
  display: flex;
  flex-direction: column;
}
.items input {
  border: none;
  border-bottom: 1px solid rgb(100,100,100);
  padding: 10px 0;  
  margin-top:20px;
  font-size: 18px;
  outline: none;
  color: rgb(100,100,100);
}
.items input:focus {
  border-bottom: 2px solid rgb(33, 150, 243);
}
.btn {
  width: 100%;
  display: block;
  border: none;
  border-radius: 3px;
  padding: 10px 25px;
  margin: 30px auto 15px;
  background-color: rgb(33, 150, 243);
  color: #fff;
  cursor:pointer;
  transition: .2s ease-in-out;
  font-size: 16px;
}
.btn:hover {
  background-color: rgb(60, 159, 240);
}
.login a {
  text-decoration: none;
  color: rgb(33, 150, 243);
  font-size: 12px;
}
</style>