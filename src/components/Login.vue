<template>
  <div class="login">
     <section class="container-fluid">
    <div class="row justify-content-center">
      <div class="col-lg-3 hagati">
        <div class="login-panel bg-white text-left">
          <fieldset>
            <h1 class="display-3 font-weight-bold">Login</h1>
            <hr />
            <form action="">
              <div class="form-group">
                <label form="email" class="input-label">Username</label>
                <input
                  type="text"
                  class="form-control"
                  placeholder="username"
                />
              </div>
              <div class="form-group">
                <label form="email" class="input-label">Password</label>
                <input
                  type="password"
                  class="form-control"
                  placeholder="password"
                />
              </div>
              <br />
              <div class="form-group d-flex justify-content-center">
                <button class="btn btn-primary btn-lg btn-block"
                    @click="login">
                  Login
                </button>
              </div>
            </form>
          </fieldset>
        </div>
      </div>
    </div>
  </section>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    login(){
      // axios post to /login
      let user = {} // response.data
      this.$emit("connected", user)
    }
  },
};
</script>

<style scoped>
.login{
  margin-left: 300px;
  height: 20px;
}
label {
  font-family: "Kaushan Script", cursive;
}
h1 {
  text-align: center;
  font-family: "Kaushan Script", cursive;
  font-style: italic;
}
.hagati{
  left: 50%;
  transform: translate(-50%, 0);
}
fieldset {
  position: relative;
  display: -ms-flexbox;
  display: flex;
  padding: 1rem;
  -ms-flex-direction: column;
  flex-direction: column;
  width: 100%;
  height: 400px;
  pointer-events: auto;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 1.1rem;
  outline: 0;
  max-width: 500px;
  box-shadow: 5px 1px 1px #0078ff;
}
button {
  border-radius: 3%;
}
.widget {
  margin: 0;
  height: unset;
}
.login-panel {
  padding: 100px 0;
  position: relative;
  .alert {
    opacity: 0;
    positon: absolute;
    top: 20px;
    width: 100%;
    &.alert-primary {
      background-color: #0078ff;
      color: #fff;
      border: none;
      font-size: 18px;
    }
    .widget {
      position: absolute;
      right: 5px;
      top: 0;
      margin: 10px;
    }
  }
}
</style>
