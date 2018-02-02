<template>
  <div id="app">
    <div id="formContainer">
      <div id="subTitle"><h4>Please Login</h4></div>
        <form id="form">
          <input type="text" placeholder="Username">
          <input type="password" placeholder="Password">
          <p>Remember me? <input type="checkbox"></p>
          <p><button id="loginBtn">Login</button><a href="#">Forgot password?</a></p>
        </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">

body {
  // background: url('https://images.unsplash.com/photo-1482192596544-9eb780fc7f66?ixlib=rb-0.3.5&s=2fd4e1abb9770bd689d2014e0d265ade&auto=format&fit=crop&w=1500&q=80');
  background: linear-gradient(to right, rgb(228, 146, 121), rgb(181, 31, 131));
}
#subTitle {
  position: absolute;
  top: 100px;
  left: 50px;
  color: #ccc;
}
#formContainer {
  // background: rgba(0,0,0,.4);
  position: relative;
  background: #333;
  width: 350px;
  height: 500px;
  margin: 100px auto;
}
#form {
  width: auto;
  padding-top: 200px;
  text-align: center;
  bottom: 0;
}
input[type="text"],
input[type="password"] {
  background: #555;
  transition: .5s all;
  width: 80%;
  border: 1px solid #ccc;
  font-size: 23px;
  outline: none;
  margin: 3px;
  color: #ccc;
    &:focus, &:active {
      outline: none;
      width: 90%;
    }
}
input[type="checkbox"] {
  // customise
}
input::placeholder {
  font-size: 20px;
}
input[type="password"] {
  color: rgb(181, 31, 131);
}
input::placeholder {
  color: #000;
}
p {
  color: #ccc;
}
button {
  margin-right: 15px;
  outline: 0;
  cursor: pointer;
  &:focus, &:active{
    outline: none;

  }
}
#loginBtn {
  background: #333;
  border: 2px solid rgb(181, 31, 131);
  width: 100px;
  border-radius: 30px;
  font-size: 20px;
  padding: 5px 10px;
  transition: .3s all;
  color: rgb(181, 31, 131);
    &:hover {
      background: rgb(181, 31, 131);
      color: #ccc;
    }
}
a {
  text-decoration: none;
  color: #ccc;
    &:hover {
      color: rgb(181, 31, 131);
      text-decoration: underline;
    }
}


</style>
