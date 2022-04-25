<template>
  <b-field :label="label">
    <b-input :value="value" @input="updateValue"> </b-input>
  </b-field>
</template>

<script>
export default {
  name: "UserName",
  props: {
    label: {
      type: String,
      default: "氏名",
    },
    value: {
      type: String,
    },
  },
  methods: {
    updateValue: function (e) {
      this.$emit("input", e.target.value);
    },
  },
};
</script>