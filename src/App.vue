<script setup>

</script>

<template>
  <el-container>
    <el-header></el-header>
    <el-main>
      <el-carousel>
        <el-carousel-item>
          <p>
            应该让el-carousel和el-main一样，走在设置了position值sticky的el-header下面
          </p>
          <p>
            如果设置el-header的z-index=11，那么会遮盖住el-scrollbar
          </p>
          <p>
            如果使用el-affix position=top又会有其他问题
          </p>
        </el-carousel-item>
      </el-carousel>
      <div class="box"></div>
    </el-main>
  </el-container>
</template>

<style>
.el-header {
  background-color: darkred;
  position: sticky;
  top: 8px;
}

.el-main {
  background-color: burlywood;
  margin: 20px;

  .el-carousel {
    width: 50dvw;
    margin: auto;

    div.el-carousel__container {
      background-color: blue;
      ;
    }

    p {
      font-weight: 900;
      color: white;
      text-align: center;
    }
  }
}

div.box {
  height: 200dvh;
}
</style>
