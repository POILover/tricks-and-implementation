<template>
  <div class="circle-btn-wrapper">
    <div class="circle-button-text">
      <span>新增组件</span>
    </div>
    <div class="circle-btn"></div>
  </div>
</template>

<script>
export default {
  name: "HoverButton"
};
</script>
<style lang="scss" scoped>
.circle-btn-wrapper {
  //   padding-bottom: 10px;
  cursor: pointer;
  position: relative;
  .circle-btn {
    height: 40px;
    width: 40px;
    background: #3370ff
      url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxOCIgaGVpZ2h0PSIxOCI+PHBhdGggZmlsbD0iI0ZGRiIgZmlsbC1ydWxlPSJldmVub2RkIiBkPSJNMTAuMTExLjExMXY3Ljc3N2g3Ljc3OHYyLjIyM0gxMC4xMXY3Ljc3OEg3Ljg5VjEwLjExbC03Ljc3OC4wMDFWNy44OWg3Ljc3N1YuMTFoMi4yMjN6Ii8+PC9zdmc+)
      no-repeat 50%;
    color: white;
    border-radius: 50%;
    border: none;
    cursor: pointer;
    position: absolute;
    top: 0;
    left: 0;
    /*box-shadow: 0 5px 10px 0 rgba(0,0,0,.2);*/
  }

  .circle-button-text {
    width: 40px;
    height: 40px;
    line-height: 40px;
    border-radius: 20px;
    padding-left: 40px;
    box-shadow: 0 5px 10px 0 rgba(0, 0, 0, 0.2);
    background: #3370ff;
    color: #fff;
    user-select: none;
    transition: width 0.3s ease-in-out;
    overflow: hidden;
    white-space: nowrap;
  }
}
.circle-btn-wrapper:hover {
  .circle-button-text {
    width: 116px;
  }
}
.circle-btn-wrapper:active {
  .circle-btn {
    background-color: #245bdb;
  }
  .circle-button-text {
    background-color: #245bdb;
  }
}
</style>
