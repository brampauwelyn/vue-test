<template>
  <div class="Header">
    <div class="innercontainer">
      <Navbar></Navbar>
      <div class="intro">
        <h1>New Era of Messaging Secure System Messaging</h1>
        <p>Chat app messaging and powerful than any other application. you can enjoy free call and free chat
        anytime and forever</p>
      </div>
      <div class="iphone">
        <img src="../assets/images/iphone.png" alt="chat app example">
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './Navbar.vue';
export default {
  components: {Navbar},
  data: function(){
    return{

    }
  }
}
</script>

<style>
.Header{
  height: 524px;
  width: 88%;
  background-image: linear-gradient(#764BA2, #667EEA);
  padding:0 6%;
  position: relative;
  overflow: hidden;
}

.intro{
  width: 550px;
  margin-top: 120px;
}

.intro h1{
  font-size: 36px;
  line-height: 44px;
  color: #fff;
  margin-bottom: 20px;
}

.intro p{
  font-size: 24px;
  line-height: 33px;
  color: #fff;
}

.iphone{
  position: absolute;
  bottom: -120px;
  right: 65px;
}

</style>
