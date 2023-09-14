<script setup>
// import{reactive, ref} from 'vue'

// const message = ref('hi')
// message.value = 'Digo'

// const titleClass = reactive({
//   counta:0
// })
// counter.counta=5
// import { RouterLink, RouterView } from 'vue-router'
import HeadBar from './components/HeadBar.vue'
import Merchant from './components/Merchant.vue'
import FootBar from './components/FootBar.vue'
import Login from './components/Login.vue'
</script>

<template>
  <div class="index">
    <HeadBar />
    <div style="display:flex ;">
      <Merchant />
      <router-view></router-view>
    </div>
    <FootBar />
  </div> 


<!-- <h1>{{ message }}</h1>
<p>
  count:{{counter.counta}}
</p> -->


 <!-- <div class="index">
<Login/>
</div> -->
  <!-- <main>
  <Login/>
</main>  -->


</template>




<style scoped>
.index {
  width: 100%;
  height: 100%;
  display: flex;
  background: #f8f6e9;
  flex-direction: column;
}
</style>
