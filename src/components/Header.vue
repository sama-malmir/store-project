<template>
    <header>
        <div class="navbar navbar-expand-lg navbar-dark d-none d-lg-block d-xl-block d-xxl-block">
            <div class="container">
                <a id="brand" class="navbar-brand" href="#Etalon" title="etalon">Etalon</a>
                <div>
                    <ul class="navbar-nav"> 
                        <li class="nav-item ">
                            <a class="nav-link " href="#home" title="home">Home</a>
                        </li>
                        <li class="nav-item ">
                            <a class="nav-link " href="#store" title="store">store</a>
                        </li>
                        <li class="nav-item ">
                            <a class="nav-link" href="#new" title="new">New</a>
                        </li>
                        <li class="nav-item ">
                            <a class="nav-link " href="#contact" title="contact">Contact</a>
                        </li>
                    </ul>
                </div>
                <div class="cart-container position-relative">
                    <span class="number-count rounded-pill py-1 px-2">{{ counterStore.count }}</span>
                    <img id="cart" src="src/assets/images/cart.svg" width="40px" alt="">
                </div>
            </div>
        </div>
        <div class="cover">
            <div class="container">
                <div class="row justify-content-center">
                    <div class="cover-details col-12 col-l-5 col-xl-5 col-xxl-5">
                        <span>2022</span>
                        <h1>Autumn Jackets</h1>
                        <h4>Autumn Sale/ Up to 50% OFF</h4>
                        <a class="btn btn-yellow text-capitalize">open collection</a>
                    </div>
                    <div class="col-12 col-md-12 col-l-6 col-xl-6 col-xxl-6 position-relative">
                        <div class="d-xxl-block d-xl-block d-l-block d-md-block d-none">
                            <img class="layer1 position-absolute" src="src/assets/images/circle-layer.svg" alt="circle-layer">
                            <img class=" layer2 position-absolute" src="src/assets/images/circle-layer.svg" alt="circle-layer">
                        </div>
                        <p id="cover-price" class="position-absolute d-none d-lg-block d-xl-block d-xxl-block">$299</p>
                        <div class="d-none d-xl-block d-xxl-block">
                            <span class="flash1 icon-flash-left"></span>
                            <span class="flash2 icon-flash-right"></span>
                        </div>
                        <picture class="cover-img position-relative " >
                            <source srcset="src/assets/images/men-with-helmet.png "  media="(min-width:768px)">
                            <source srcset="src/assets/images/Group 2.svg" >
                            <img src="src/assets/images/Group 2.svg" alt="men-with-helmet">
                        </picture>
                        <img class="off position-absolute d-none d-lg-block d-xl-block d-xxl-block" src="src/assets/images/off.svg" alt="%off">
                    </div>
                    <div class="circles position-relative col-12 col-l-1 col-xl-1 col-xxl-1 m-auto">
                        <a href="#"><div class="circle1"></div></a>
                        <a href="#"><div class="circle2"></div></a>
                        <a href="#"><div class="circle3"></div></a>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>
<script>
    import { useCounterStore } from '../router/stores/counter';
    import { mapStores } from 'pinia';
    export default{
        computed:{
            ...mapStores(useCounterStore)
        }
    }
</script>