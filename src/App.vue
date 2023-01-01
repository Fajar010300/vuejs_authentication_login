<template>
  <div id="app">
    <h1>{{ NavComponent }}</h1>
    <div class="auth-wrapper">
      <div class="auth-inner">
        <HomeComponent />
      </div>
    </div>
  </div>
</template>

<script>
import NavComponent from "./components/NavComponent.vue";
import HomeComponent from "./components/HomeComponent.vue";
export default {
  name: "App",
  component: {
    NavComponent,
    HomeComponent,
  },
};
</script>

<style>
/* @import url(<linkrel="stylesheet"href="https://fonts.googleapis.com/css?family=Tangerine">); */

* {
  box-sizing: border-box;
}

body {
  background-color: #ec355a;
  min-height: 100vh;
  display: flex;
  font-weight: 400;
  font-family: Arial, Helvetica, sans-serif;
}

.navbar-brand {
  text-align: center;
  color: black;
}

h1,
h2,
h3,
h4,
h5,
h6,
label,
span {
  font-weight: 500;
  font-family: Arial, Helvetica, sans-serif;
}

body,
html,
#app,
#root,
.auth-wraper {
  width: 100%;
  height: 100%;
}

#app {
  text-align: center;
}

.navbar-light {
  background-color: #ffffff;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
}
.auth-wraper {
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: left;
}
.auth-inner {
  width: 500px;
  margin: auto;
  background: #ffffff;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
  padding: 100px 75px 200px 80px;
  border-radius: 15px;
  transition: all 0.3s;
}

.auth-wraper .form-control:focus {
  border-color: black;
  box-shadow: none;
}
.auth-wraper h3 {
  text-align: center;
  margin: 0;
  line-height: 1;
  padding-bottom: 20px;
}

.custom-control-label {
  font-weight: 400;
}
.forgot-password a {
  text-align: right;
  font-size: 13px;
  padding-top: 10px;
  color: blue;
  margin: 0;
}

.forgot-password a {
  color: red;
}
</style>
