<template lang="html">
    <div >
        <Header/>
        <Slider/>
        
        <Footer cname="mfooter"/>
        <Navbar/>
    </div>
</template>
 
<script>
    import Header from '../public/header.vue'
    import Footer from '../public/footer.vue'
    import Navbar from '../public/navbar.vue'
    import Slider from './rslider.vue'

    export default {
        components:{
            Header,
            Slider,
            Footer,
            Navbar,
        }
    }
</script>

<style lang="scss" module>
   .mfooter{
    margin-top:0;
      ul{
        li:first-child{
            display:none;
        }
      }
   }
</style>
