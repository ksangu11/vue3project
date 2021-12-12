<template>
    <div class="photocontainer">
        <div id= "tagline">
            <h3>Hover over the images to see Bear's puppy photos</h3>
        </div> 
        <div class="photo">
            <img :src="pictureHover1" class="hoverEffect" @mouseover="hover= true" @mouseleave="hover=false">
            <img :src="pictureHover2" class="hoverEffect" @mouseover="hover= true" @mouseleave="hover=false">
            <img :src="pictureHover3" class="hoverEffect" @mouseover="hover= true" @mouseleave="hover=false">
            <img :src="pictureHover4" class="hoverEffect" @mouseover="hover= true" @mouseleave="hover=false">
            
        </div>    
    </div>
</template>

<script>

export default{
    name: 'Gallery',
    data () {
        return {
            pictureStatic1: require("@/assets/bearadult1.jpg"),
            pictureAfter1: require("@/assets/bearpuppy1.jpg"),
            pictureStatic2: require("@/assets/bearadult2.jpg"),
            pictureAfter2: require("@/assets/bearpuppy2.jpg"),
            pictureStatic3: require("@/assets/bearadult3.jpg"),
            pictureAfter3: require("@/assets/bearpuppy3.jpg"),
            pictureStatic4: require("@/assets/bearadult4.jpg"),
            pictureAfter4: require("@/assets/bearpuppy4.jpg"),
            hover: false
        }
    },
    computed: {
        pictureHover1(){
            if(this.hover == true) {
                return this.pictureAfter1
            } else{
                return this.pictureStatic1
            }
        },
        pictureHover2(){
            if(this.hover == true) {
                return this.pictureAfter2
            } else{
                return this.pictureStatic2
            }
        },
        pictureHover3(){
            if(this.hover == true) {
                return this.pictureAfter3
            } else{
                return this.pictureStatic3
            }
        },
        pictureHover4(){
            if(this.hover == true) {
                return this.pictureAfter4
            } else{
                return this.pictureStatic4
            }
        },
    },
};

</script>

<style scoped>
    .photocontainer {
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
        padding: 10px;
    }
    .photo{
        margin-left: 0 auto;
        margin-right: 0 auto;
    }
    img {
        width: 40%;
        display: inline-flexbox;
        margin: 5%;
        
    }
    h3{
       margin-left: auto; 
       margin-right: auto;
       text-align: center;
    }
</style>
