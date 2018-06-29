<template>
  <div class="login">
    <el-card class="box-card">
      <div slot="header" class="clearfix">
        <span>用户登入</span>
      </div>
      <el-form ref="form" :model="form" label-width="80px" label-position="top">
        <el-form-item label="用户名称">
          <el-input v-model="form.name"></el-input>
        </el-form-item>
        
        <el-form-item label="用户密码">
          <el-input v-model="form.password"></el-input>
        </el-form-item>
        
        <el-button class="login_button" type="primary">登入</el-button>
      </el-form>
    </el-card>
  </div>
</template>

<script>
  export default {
    name: 'Login',
    data() {
      return {
        form: {
          name: "",
          password: ""
        }
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .login {
    margin: 0;
    padding: 0;
    height: 100%;
    width: 100%;
    display: flex;
  }
  
  .login .box-card {
    margin: 150px auto;
    width: 450px;
    height: 380px;
  }
  
  .login_button {
    width: 100%;
    margin-top: 7px;
  }

</style>
