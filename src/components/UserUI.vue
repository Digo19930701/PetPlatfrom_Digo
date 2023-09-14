<template>
  <!-- Form -->
  <div class="login">
    <el-form :model="loginForm" class="loginForm">
      <el-form-item label="姓名" :label-width="formLabelWidth">
        <el-input v-model="loginForm.account" autocomplete="off"></el-input>
      </el-form-item>
      <el-form-item label="電話" :label-width="formLabelWidth">
        <el-input v-model="loginForm.password" autocomplete="off" />
      </el-form-item>
      <el-form-item label="Email" :label-width="formLabelWidth">
        <el-input v-model="loginForm.password" autocomplete="off" />
      </el-form-item>
      <el-form-item label="地址" :label-width="formLabelWidth">
        <el-input v-model="loginForm.password" autocomplete="off" />
      </el-form-item>
      <el-form-item label="生日" :label-width="formLabelWidth">
        <el-input v-model="loginForm.password" autocomplete="off" />
      </el-form-item>
      <el-form-item label="身分證" :label-width="formLabelWidth">
        <el-input v-model="loginForm.password" autocomplete="off" />
      </el-form-item>

      
    </el-form>





    

    

    
  </div>
</template>

<script lang="ts" setup>
import { reactive, ref } from 'vue'

const dialogFormVisible = ref(false)
const formLabelWidth = '100px'

const form = reactive({
  name: '',
  phone: '',
  mail: '',
  address: '',
  bithday: '',
  id: '',
  account: '',
  password: '',
  passwordAgain: ''
})

const loginForm = reactive({
  account: '',
  password: ''
})
const login = () => { }

const value1 = ref(true)
const value2 = ref(true)
const value3 = ref(true)
const value4 = ref(true)
const value5 = ref(true)
const value6 = ref(true)
</script>



<style scoped>
.login {
  text-align: center;
  top: 50%;
}

.loginForm {
  display: inline-block;
  vertical-align: middle;
}

.el-button--text {
  margin-right: 15px;
}

.el-select {
  width: 300px;
}

.el-input {
  width: 300px;
}

.dialog-footer button:first-child {
  margin-right: 10px;
}
</style>
