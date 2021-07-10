<template>
<div>
  <p>いいね({{ totalNumber / 2 }})</p>
  <button @click="increment">+1</button>
</div>
</template>

<script>
export default {
  props: ["totalNumber"],
  computed: {
    halfNumber() {
      return this.totalNumber /2;
    }
  },

  methods: {
      increment: function() {
          this.$emit("my-click", this.totalNumber + 1);
      }
  }
};
</script>

<style scoped>

 div {
   border: 1px solid blue;
 }

</style>

