<template>
  <div>
    首页
    <van-cell-group>
      <van-cell title="单元格" value="内容" />
      <van-cell title="单元格" value="内容" />
      <van-button color="#7232dd">单色按钮</van-button>
    </van-cell-group>
    <div class="login">
      <van-button type="primary" @click="goLogin">跳转登录页</van-button>
    </div>
  </div>
</template>

<script setup="props">
import { useRouter } from "vue-router";
const router = useRouter();
const goLogin = () => {
  router.push("/login");
};
</script>

<style lang='scss' scoped>
</style>