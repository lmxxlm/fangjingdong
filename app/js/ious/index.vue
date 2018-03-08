<template lang="html">
    <div >
        <Header/>
        <Slider/>
        <Welfare/>
        <Servise/>
        <Footer/>
        <Navbar/>
    </div>
</template>

<script>
    import Header from '../public/header.vue'
    import Footer from '../public/footer.vue'
    import Navbar from '../public/navbar.vue'
    import Slider from './iSlider.vue'
    import Welfare from './welfare.vue'
    import Servise from './service.vue'
   
    export default {
        components:{
            Header,
            Slider,
            Footer,
            Navbar,
            Welfare,
            Servise
        }
    }
</script>

<style lang="scss" module>

</style>
