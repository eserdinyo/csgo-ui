<template>
  <div class="Sidebar">
    <div class="Sidebar_logo">
      <img src="../assets/logo.png" alt="" />
    </div>
    <icon-play class="icon" />
    <icon-gun class="icon1" />
    <icon-tv class="icon1" />
    <icon-settings class="icon1" />
    <icon-close class="icon1" style="margin-top: auto" />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.Sidebar {
  width: 80px;
  height: 100vh;
  backdrop-filter: blur(8px);
  display: flex;
  flex-direction: column;
  align-items: center;
  border-right: 1px solid #ededed38;
  padding-bottom: 20px;
  &_logo {
    border-bottom: 1px solid #ededed38;
    padding: 22px 15px;
    img {
      width: 100%;
      filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(93deg)
        brightness(103%) contrast(103%);
    }
  }

  .icon {
    height: 50px;
    margin-top: 25px;
    fill: #171717;
  }

  .icon1 {
    height: 30px;
    margin-top: 60px;
  }
}
</style>
