<template>
    <div :class="$style.header">
        <span :class="$style.left">
            <em>登陆</em>&nbsp;|&nbsp;<em>注册</em>
        </span>
        <btn :class="$style.downLoad">下载app</btn>
    </div>
</template>

<script>
   import btn from '../core/btn.vue'

    export default {
        components:{
            btn
        }
    }
</script>

<style lang="scss" module>
    .header{
        color:#666;
        height:100px;
        line-height:100px;
        z-index:100;
        position:fixed;
        top:0;
        left:0;
        right:0;
        font-size:32px;
        background:#fff url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
        background-size:auto 50%;
        .left{
            font-size:28px;
            height:30px;
            line-height: 30px;
            margin:17px 0 0 18px;
        }
        .downLoad{
            float:right;
            font-size: 20px;
            border-width: 0;
            height: 56px;
            line-height: 56px;
            min-width: 120px;
            padding: 0;
            -webkit-border-radius: 4px;
            -moz-border-radius: 4px;
            border-radius: 4px;
            margin: 28px 24px 0 0;


        }


    }

</style>