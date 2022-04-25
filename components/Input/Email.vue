<template>
  <b-field :label="label">
    <b-input v-model="email" type="email"></b-input>
  </b-field>
</template>

<script>
export default {
  name: "Email",
  props: {
    label: {
      type: String,
      default: "メールアドレス",
    },
  },
  data() {
    return {
      email: "",
    };
  },
};
</script>