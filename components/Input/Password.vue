<template>
  <b-field :label="label">
    <b-input v-model="password" type="password"></b-input>
  </b-field>
</template>

<script>
export default {
  name: "Password",
  props: {
    label: {
      type: String,
      default: "パスワード",
    },
  },
  data() {
    return {
      password: "",
    };
  },
};
</script>