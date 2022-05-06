<template>
<div>
<Nav></Nav>
<Category></Category>
<Swiper></Swiper>
</div>
</template>

<script>
import Nav from './components/xm-nav.vue'
import Category from './components/xm-nav-category.vue'
import Swiper from './components/xm-swiper.vue'
export default {
  data () {
    return {
}
  },
components: {
  Nav,
  Category,
  Swiper
}
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
</style>
