<template>
  <div>
    <h1>Layout Too</h1>
    <slot/>
    <LatestPost v-if="latest"/>
  </div>
</template>

<script>
import LatestPosts from "../components/LatestPosts.vue";
export default {
  components: {
    LatestPosts
  },
  props: ["latest"]
};
</script>
