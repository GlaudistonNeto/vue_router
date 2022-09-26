<template>
  <div class="test">
    <input type="email" name="email" placeholder="Email"><br>
    <input type="text" name="name" placeholder="Name"><br>
    <h4>{{ routeParameter }}</h4>
    <button>Test</button>
    <router-view />
  </div>
</template>

 <script>
export default {
  created() {
    this.routeParameter = this.$route.params.data;
  },
  data() {
    return {
      routeParameter: 'Nothing'
    }
  }
}
</script>
