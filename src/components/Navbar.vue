<template>
  <div class="Navbar cf">
    <a class="logo" href="/">{{title}}</a>
    <ul class="navlinks">
      <li v-for="link in links">
        <a :href="link.url">{{link.name}}</a>
      </li>
    </ul>
  </div>
</template>


<script>
export default {
  data: function(){
    return{
      title: 'Chatapp',
      links: [
        {
          url: '/feature',
          name: 'feature'
        },
        {
          url: '/how-to',
          name: 'how it works'
        },
        {
          url: '/download',
          name: 'download'
        }
      ]
    }
  }
}
</script>


<style>

.Navbar{
  padding-top: 25px;
}

.Navbar a.logo{
  font-family: 'Montserrat', sans-serif;
  font-weight: 500;
  font-size: 32px;
  line-height: 39px;
  color: #fff;
  text-decoration: none;
  display: block;
  float: left;
  margin-right: 58px;
}

.navlinks{
  padding: 0;
  display: block;
  float: left;
}

.navlinks li{
  display: block;
  float: left;
}

.navlinks li a{
  text-decoration: none;
  color: #fff;
  margin-right: 48px;
  font-size: 18px;
  padding: 7px 0;
  line-height: 39px;
  text-transform: capitalize;
}

</style>
