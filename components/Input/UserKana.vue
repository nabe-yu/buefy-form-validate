<template>
  <b-field :label="label">
    <b-input v-model="userKana"></b-input>
  </b-field>
</template>

<script>
export default {
  name: "UserKana",
  props: {
    label: {
      type: String,
      default: "カナ氏名",
    },
  },
  data() {
    return {
      userKana: "",
    };
  },
};
</script>