<template>
<div>
  <LikeHeader>
    
  </LikeHeader>
  <LikeNumber :total-number="number" v-on:my-click="number = $event"></LikeNumber>
  <LikeNumber :total-number="number"></LikeNumber>
</div>
</template>


<script>
import LikeHeader from "./components/LikeHeader.vue";
export default {
  data() {
    return {
      number: 10
  };
  },
  components: {
    LikeHeader
  }
}
</script>
