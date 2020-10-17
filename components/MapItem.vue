<template>
  <div class="MapItem" :class="{ MapItem_active: isActive }" @click="toggleMap">
    <div class="MapItem_title">Mirage</div>
    <div class="MapItem_footer">
      <icon-time class="icon" />
      <span>Wait Time 03:06</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: false,
    }
  },
  methods: {
    toggleMap() {
      this.isActive = !this.isActive
    },
  },
}
</script>

<style lang="scss" scoped>
.MapItem {
  user-select: none;
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.5)),
    url('../assets/maps/mirage.jpeg');
  background-position: center;
  background-size: cover;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  display: flex;
  flex-direction: column;
  cursor: pointer;
  border-radius: 2px;

  &_active {
    border: 8px solid #fff;
    box-shadow: rgba(255, 255, 255, 0.803) 0px 0px 24px;
  }

  &_title {
    margin-top: auto;
    color: #fff;
    text-align: center;
    font-size: 20px;
    font-weight: 600;
  }

  &_footer {
    display: flex;
    justify-content: center;
    color: #fff;
    align-items: center;
    padding: 16px 0;
    padding-bottom: 20px;
    font-size: 12px;
    font-weight: 600;
  }

  .icon {
    width: 14px;
    margin-right: 10px;
  }
}
</style>
