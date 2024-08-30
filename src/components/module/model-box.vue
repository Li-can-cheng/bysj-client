<template>
    <div class="subtitle-modelbox-widget">
        <div class="titile-container">
            <div class="section-title">
                {{title}}
                <!-- <a :href="link" class="more-link">更多</a> -->
                <router-link :to="link" class="more-link">更多
                </router-link>
            </div>
        </div>
        <div class="sidebar-widget-body">
            <slot>
            </slot>
        </div>
        <!-- /.sidebar-widget-body -->
    </div>
</template>
<style type="text/scss" scoped lang="scss">
    .subtitle-modelbox-widget {
        background-color: #fff;
        box-shadow: 0 2px 4px 0 rgba(0,0,0,.08);
        .section-title {
            // font-size: 20px;
            // font-family: 'Open Sans', sans-serif;
            // border-bottom: 1px solid #e3e3e3;
            // padding-bottom: 10px;
            // color: #4694c5;
            // text-transform: uppercase;
            // font-weight: bold;
            // margin-top: 0px;
            // padding-left: 20px;
            // padding-top: 20px;
            display: flex; /* 启用Flexbox布局 */  
            align-items: center; /* 垂直居中子元素 */  
            font-size: 20px;  
            font-family: 'Open Sans', sans-serif;  
            border-bottom: 1px solid #e3e3e3;  
            padding-bottom: 10px;  
            color: #4694c5;  
            padding-top:10px;
            text-transform: uppercase;  
            font-weight: bold;  
            margin-top: 0px;  
            padding-left: 20px;

            // padding-left: 10px;
        }
        .more-link{
            text-decoration: none;
            color:rgb(151, 151, 164);
            font-size: 18px;
            padding-right: 26px;
            padding-top:4px;
            margin-left: auto;
        }
        .sidebar-widget-body{
            padding: 20px;
        }
    }
    .title-container {  
    display: flex;  
    justify-content: space-between;  
    align-items: center; /* 如果需要垂直居中 */  
    }  
    .more-link{
        text-align: right;
    }

</style>
<script>
    export default {
        name: "e-module-model-box",
        data() {
            return {

            }
        },
        props:{
            title:String,
            link:String
        },
        watch: {},
        computed: {

        },
        methods: {},
        created() {
        },
        mounted() {
        },
        destroyed() {
        }
    }
</script>
