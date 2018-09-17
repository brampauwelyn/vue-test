<template>
  <div class="feature-container cf">
    <h2>Feature</h2>
    <div class="feature " v-for="feature in features">
      <img :src="feature.img" alt="">
      <h3>{{feature.title}}</h3>
      <p>{{feature.text}}</p>
    </div>
  </div>
</template>

<script>
export default {
  data: function(){
    return{
      features: [
        {
          img: require('../assets/images/features/privacy.png'),
          title: 'privacy',
          text: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
        },
        {
          img: require('../assets/images/features/secure.png'),
          title: 'secure',
          text: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
        },
        {
          img: require('../assets/images/features/connect.png'),
          title: 'connect',
          text: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry.'
        }
      ]
    }
  }
}
</script>

<style>

.feature-container{
  width: 88%;
  margin: 0 auto;
  padding: 50px 0;
}

.feature-container h2{
  text-align: center;
  color: #434343;
  font-size: 36px;
  margin-bottom: 58px;
}

.feature{
  text-align: center;
  width: 395px;
  display: block;
  float: left;
}

.feature img{
  margin-bottom: 30px;
  width: 50%;
}

.feature h3{
  font-size: 30px;
  color: #434343;
  text-transform: capitalize;
  margin-bottom: 10px;
}

.feature p{
  font-size: 18px;
  line-height: 33px;
}


</style>

