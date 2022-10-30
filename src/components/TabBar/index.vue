<template>
  <footer id="footer">
    <ul>
      <router-link to="/movie" custom v-slot="{ navigate,isActive }">
        <li @click="navigate" :class="isActive?'activeRoute':''">
          <span class="iconfont icon-quanpiao"></span>
          <p>电影</p>
        </li>
      </router-link>

      <router-link to="/cinema" custom v-slot="{ navigate,isActive }">
        <li @click="navigate" :class="isActive?'activeRoute':''">
          <span class="iconfont icon-shipin"></span>
          <p>影院</p>
        </li>
      </router-link>

      <router-link to="/mine" custom v-slot="{ navigate,isActive }">
        <li @click="navigate" :class="isActive?'activeRoute':''">
          <span class="iconfont icon-wode"></span>
          <p>我的</p>
        </li>
      </router-link>
    </ul>
  </footer>
</template>
<script>
export default {
  name: 'TabBar'
}
</script>
<style lang="scss" scoped>
#footer {
  width: 100%;
  height: 50px;
  background: white;
  border-top: 2px #ebe8e3 solid;
  position: fixed;
  left: 0;
  bottom: 0;
  ul {
    display: flex;
    text-align: center;
    height: 50px;
    align-items: center;
    li {
      flex: 1;
      span {
        font-size: 20px;
      }
      p {
        font-size: 12px;
      }
    }
    li.activeRoute {
      color: rgb(254, 165, 0);
    }
  }
}
</style>
