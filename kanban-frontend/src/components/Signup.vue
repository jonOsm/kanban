<template>
  <div class="signup-page">
    <div class="container">
      <div class="columns">
        <div class="column is-one-third">
          <div class="card">
            <div class="card-content">
              <div calss="content">
                <p class="title">Sign Up</p>
                <div class="field">
                  <label class="label">Email</label>
                  <div class="control has-icons-left has-icons-right">
                    <input
                      class="input"
                      type="text"
                      placeholder="example@email.com"
                      v-model="email"
                    />
                    <span class="icon is-small is-left">
                      <i class="fas fa-envelope"></i>
                    </span>
                    <span class="icon is-small is-right">
                      <i class="fas fa-check"></i>
                    </span>
                  </div>
                </div>
                <div class="field">
                  <label class="label">Username</label>
                  <div class="control has-icons-left has-icons-right">
                    <input class="input" type="text" placeholder="kanbanuser1" v-model="username" />
                    <span class="icon is-small is-left">
                      <i class="fas fa-user"></i>
                    </span>
                    <span class="icon is-small is-right">
                      <i class="fas fa-check"></i>
                    </span>
                  </div>
                </div>
                <div class="field">
                  <label class="label">Password</label>
                  <div class="control has-icons-left has-icons-right">
                    <input class="input" type="password" v-model="password" />
                    <span class="icon is-small is-left">
                      <i class="fas fa-lock"></i>
                    </span>
                    <span class="icon is-small is-right">
                      <i class="fas fa-check"></i>
                    </span>
                  </div>
                </div>
                <div class="field">
                  <label class="checkbox">
                    <input type="checkbox" v-model="tocAccepted" />
                    I agree to the
                    <a href="#">terms and conditions</a>
                  </label>
                </div>

                <div class="field is-clearfix">
                  <div class="control is-pulled-right">
                    <button class="button is-link" @click="signup">Submit</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return { email: "", username: "", password: "", tocAccepted: "" };
  },
  methods: {
    signup() {
      console.log(this.email);
      console.log(this.username);
      console.log(this.password);
      console.log(this.tocAccepted);
    },
  },
};
</script>

<style>
.signup-page {
  background-color: slategrey;
  position: absolute;
  width: 100%;
  height: 100vh;
}
.columns {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>