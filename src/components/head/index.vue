<template>
  <div class="haed">
    <div class="headNav">
      <a class="reset">
        <img src="../../assets/reset.png" alt="">
      </a>
      <div class="p">口碑下载站</div>
      <div
        class="menu"
        :style="{
          backgroundPositionY:
            isMenu
              ? '0px'
              : '34px'
        }"
        @click="isMenu = !isMenu"
      ></div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      isMenu: true
    }
  }
}
</script>

<style lang="scss" scoped>
.headNav {
  width: 100%;
  height: 50px;
  background-color: #68c875;
  line-height: 50px;
  position: relative;
  .p {
    font-size: 20px;
    text-align: center;
    font-weight: bold;
    color: #fff;
  }
  .reset {
    width: 42px;
    height: 38px;
    display: block;
    position: absolute;
    left: 10px;
    top: 50%;
    transform: translateY(-50%);
    overflow: hidden;
    img {
      width: 100%;
      height: 100%;
      position: relative;
      top: -10px;
    }
  }
  .menu {
    width: 34px;
    height: 34px;
    overflow: hidden;
    position: absolute;
    right: 10px;
    top: 50%;
    transform: translateY(-50%);
    background: url('../../assets/menu.png');
    background-size: 34px;
  }
}
</style>
