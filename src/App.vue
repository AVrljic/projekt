<template>
    <div class="app">
      <Navbar />
      <div>
         <Carousel >
            <carousel-slide v-for="slide in slides" :key="slide" class="carousel-slider">
                <img :src="slide" :alt="slide">
            </carousel-slide>
        </Carousel>
      </div>
      <Footer />  
    </div>    
</template>

<script>
import Navbar from './components/Navbar';
import Carousel from './components/Carousel';
import CarouselSlide from './components/CarouselSlide';
import Footer from './components/Footer';
export default {
    name: 'App',
    data(){
        return {
            slides: [
                'https://picsum.photos/id/1006/600/300',
                'https://picsum.photos/id/1016/600/300',
                'https://picsum.photos/id/1015/600/300',
                'https://picsum.photos/id/1021/600/300',
                'https://picsum.photos/id/1045/600/300',
                
            ]
        }
    },
    components : {
        Navbar,
        Carousel,
        CarouselSlide,
        Footer
    }
}
</script>

<style>

    .app {
        
        justify-content: center;
    }
    .carousel {
        position:center;
        overflow: hidden;
        width:800px;
        height:500px;
        z-index:10;
    }
    .btn {
        padding:5px 10px;
        background-color:rgba(0,0,0,0.5);
        border:1px solid transparent;
        margin:5px 10px;
        color:#FFF;
        height:50px;
        width:50px;
        position:absolute;
        margin-top:-25px;
        z-index:2;
    }
    .btn:hover {
        cursor: pointer;
    }
    .btn:focus{
        outline:none;
    }
    .btn-next {
        top:50%;
        right:0;
    }
    .btn-prev {
        top:50%;
        left:0;
    }
    .carousel-slider {
        position:absolute;
        top:0;
        left:0;
        bottom:0;
        right:0;
    }
    .carousel-slider img {
        width:100%;
        height:100%;
    }
</style>
