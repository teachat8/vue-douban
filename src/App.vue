<template>
    <!--主页-->
    <div id="app">
        <!--头部-->
        <Vheader></Vheader>
        <!--渲染区-->
        <transition enter-active-class="animated flipInY">
            <!--保持状态不重复发送请求-->
            <!--<keep-alive>-->
            <router-view></router-view>
            <!--</keep-alive>-->
        </transition>

    </div>
</template>

<script>
    //    导入头部
    import Vheader from './components/common/Header.vue'

    export default {
        name: 'app',
        data() {
            return {}
        },
        methods: {},
        components: {
            Vheader
        }

    }
</script>
<style>
    @import "assets/css/Init.css";
    #app {
        padding-top: 47px;
        max-width: 650px;
        background: #fff;
        margin: 0 auto;
        overflow-x: hidden;
        overflow-y: hidden;
    }
</style>
