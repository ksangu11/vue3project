<template>
<div class="container">
  <Header />
  <Gallery />
  <Button text="Reach Out"/>
</div>
</template>

<script>
import Header from './components/header.vue'
import Button from './components/button.vue'
import Gallery from './components/gallery.vue'

export default {
  name: "App",
  components: {
    Header,
    Button,
    Gallery
  },

};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Quicksand&display=swap');
body{
  font-family: 'Quicksand', sans-serif;
  background-image: url("assets/bluepawprints.jpg")
}
.container{
  max-width: 70%;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 3px solid steelblue;
  border-radius: 10px;
  background: rgb(238, 246, 248);
}
.btn{
  display: inlne-block;
  background: rgb(4, 41, 77);
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
  box-shadow: lightslategrey;
}
.btn:focus{
  outline: none;
}
.btn:active{
  transform: scale(0.98);
}
.btn-block{
  display: block;
  width: 100%;
}
</style>
