<template>
  <section class="section">
    <div class="columns">
      <div class="column is-4"></div>
      <div class="column is-4 box">
        <my-input
          v-model="inputResult.userName"
          placeholder="サンプル"
          name="sample-input"
          type="text"
        ></my-input>
        <user-name v-model="inputResult.userName"></user-name>
        <user-kana></user-kana>
        <email></email>
        <password></password>
        <div class="has-text-centered">
          <b-button class="is-primary">Submit</b-button>
        </div>
      </div>
      <div class="column is-4">{{ userName }}</div>
    </div>
  </section>
</template>

<script>
import UserName from "../components/Input/UserName.vue";
import UserKana from "../components/Input/UserKana.vue";
import Email from "../components/Input/Email.vue";
import Password from "../components/Input/Password.vue";
import MyInput from "../components/Input/MyInput.vue";
export default {
  name: "IndexPage",
  components: {
    UserName,
    UserKana,
    Email,
    Password,
    MyInput,
    UserName,
  },
  data() {
    return {
      inputResult: {
        userName: "",
      },
    };
  },
};
</script>