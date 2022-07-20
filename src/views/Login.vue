<template>
  <dev>
    <el-form ref="form" :model="form">
        <el-form-item label="账号">
            <el-input type="text" placeholder="请输入用户名" v-model="form.name"></el-input>
        </el-form-item>
        <el-form-item label="密码">
            <el-input type="password" placeholder="请输入密码" v-model="form.password"></el-input>
        </el-form-item>
        <el-form-item>
            <el-button type="primary" @click="onSubmit">登录</el-button>
        </el-form-item>
    </el-form>
  </dev>
</template>

<script>
export default {
  name: "Login",
  data(){
    return{
        form:{
            name:'',
            password:''
        }
    }
  },
  methods:{
    onSubmit(){
        alert("Hello");
    }
  }
};
</script>

<style>
</style>


