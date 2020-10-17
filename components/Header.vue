<template>
  <div class="Header">
    <div class="Header_logo">PLAY</div>
    <div class="Header_nav">
      <nuxt-link to="/"> Competitive </nuxt-link>
      <nuxt-link to="/a"> Casual </nuxt-link>
      <nuxt-link to="/v"> Deatchmatch </nuxt-link>
      <nuxt-link to="/c"> War Games </nuxt-link>
      <nuxt-link to="/d"> Wingman </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.Header {
  width: 100%;
  border-bottom: 1px solid #ededed38;
  backdrop-filter: blur(8px);
  color: #c5d0d0;
  font-weight: 500;
  font-size: 20px;
  letter-spacing: 1px;

  &_logo {
    padding: 25.5px 25px;
  }

  &_nav {
    display: flex;
    align-items: center;
    padding-left: 25px;
    border-top: 1px solid #ededed38;

    a {
      font-size: 14px;
      color: #fff;
      text-decoration: none;
      margin-right: 30px;
      padding: 13px 2px;
      padding-top: 17px;
    }

    .nuxt-link-active {
      border-bottom: 4px solid #ffffff;
    }
  }
}
</style>
