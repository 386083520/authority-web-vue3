<template>
  <div class="login">
    <el-form class="login-form">
      <h3 class="title">若依后端管理系统</h3>
      <el-form-item>
        <el-input placeholder="账号"></el-input>
      </el-form-item>
      <el-form-item>
        <el-input placeholder="密码"></el-input>
      </el-form-item>
      <el-form-item>
        <el-input
            placeholder="验证码"
            style="width: 63%"
        ></el-input>
        <div class="login-code">
          图片
        </div>
      </el-form-item>
      <el-checkbox style="margin: 0px 0px 25px 0px">记住密码</el-checkbox>
      <el-form-item>
        <el-button
            style="width: 100%"
            type="primary"
            size="large"
        >
          登录
        </el-button>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  name: "login"
}
</script>

<style scoped lang="scss">
.login {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  background-image: url("../assets/images/login-background.jpg");
  background-size: cover;
}
.login-form {
  background: #fff;
  width: 400px;
  padding: 25px 25px 5px 25px;
  border-radius: 6px;
  .title {
    text-align: center;
    color: #707070;
    margin: 0px auto 30px auto;
  }
  .login-code {
    width: 33%;
  }
}
</style>