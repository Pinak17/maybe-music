<template>
  <div>
    <h1>Register</h1>
    <input type="email" name="email" v-model="email" placeholder="email" />
    <br>
    <input type="password" name="password" v-model="password" placeholder="password" />
    <br>
    <button @click="register">Register</button>
  </div>
</template>

<script>
// import AuthenticationService from '@/services/authenticationService'
export default {
  data () {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    /* async register () {
      const response = await AuthenticationService.register({
        email: this.email,
        password: this.password
      })
    } */
    register () {
      console.log('register button got clicked', this.email)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
