<template>
    <article>
        <Slider :items="items" :cname="$style.slider"></Slider>
        <section :class="$style.list">
            <div :class="$style.item" v-for="item in enters" :key="item.img">
                <router-link :to="{name:item.href}">
                    <img :src="item.img" alt="item.title">
                    <h4>{{item.title}}</h4>
                </router-link>
            </div>
        </section>
    </article>
</template>

<script>
    import Slider from '../core/slider.vue'

    export default {
        components:{
            Slider
        },
        data(){
            return {
                items:[
                    {
                        href:"home1",
                        src:"//img12.360buyimg.com/jrpmobile/jfs/t19234/146/484647810/42715/ee6a513f/5a86e090N12c1a4f0.jpg?width=750&height=320"
                    },
                    {
                        href:"home2",
                        src:"//img12.360buyimg.com/jrpmobile/jfs/t17980/53/468304775/37826/1ec13ed0/5a86e0ddN7efa41cc.jpg?width=750&height=320"
                    },
                    {
                        href:"home3",
                        src:"//img12.360buyimg.com/jrpmobile/jfs/t19060/119/496305784/34918/f1cf2485/5a86e053Nc2a30260.jpg?width=750&height=320"
                    }
                ],
                enters:[
                    {
                        href:'home',
                        img:"//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132",
                        title:"优惠券"
                    },
                    {
                        href:'home',
                        img:"//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132",
                        title:"领红包"
                    },{
                        href:'home',
                        img:"//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132",
                        title:"抢钢蹦"
                    },{
                        href:'home',
                        img:"//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135",
                        title:"白条提额"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .slider{
        margin-top:120px;
        img{
            width:100%;
        }
    }
    .list{
        @include list(row);
        background:#fff;
        padding-top:40px;
        padding-bottom:20px;
        justify-content: space-around;
        a{
            text-decoration: none;
        }
        .item{
            text-align:center;
            img{
                display:inline-block;
                width:90px;
                height:90px;
            }
            h4{
                font-size:26px;
                margin-top:12px;
                color:#666;
            }
        }
    }
</style>