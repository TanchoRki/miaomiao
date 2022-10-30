<template>
  <div id="main">
    <Header />
    <tab-bar />
  </div>
</template>
<script>
import Header from '@/components/Header'
import TabBar from '@/components/TabBar'
export default {
  name: 'Movie',
  components: {
    TabBar,
    Header
  }
}
</script>
<style lang="scss" scoped>

</style>
