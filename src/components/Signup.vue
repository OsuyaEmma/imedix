<template>
  <main>
    <div>
      <h1>Medix Ultimate</h1>
      <h2>Version 3.5</h2>       
      <p>Hospital Information management and accounting software</p>
{{username}}
{{password}}
      <form @submit.prevent="signup">
        <div>
          <p style="font-family: Elephant; color: #008000;">User Name
          <input type="text" v-model="username" placeholder="Username" required />
          </p>
        </div>
        <div>
          <p>password</p>
          <p style="font-family: Elephant; color: #008000;">Password
          <input type="password" v-model="password" placeholder="Password" required />
        </p>
        </div>
        <div>
          <button type="submit">
            Login
          </button>
        </div>
      </form>
    </div>
  </main>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      password: "",
    };
  },
  methods: {
    signup() {
      console.log(this.username, this.password);
    },
  },
};
</script>

<style></style>
