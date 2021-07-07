/* 
    当前.vue文件不是一个组件，而是一个组件的基本配置
 */

/* 配置组件模板结构 */
<template>
    <div>
        <h2 class="name">学校名：{{name}}</h2>
        <h2 class="address" @click="showInfo">地址：{{address}}</h2>
    </div>
</template>>

/* 配置组件数据、交互、事件 */
<script>
    //此处只是暴露了一个组件的配置，并没有去创建组件（只是准备了信息）
    //因为没有调用vue.extend
    export default{
        //data中存放组件需要的数据
        data(){
            return{
                name:'振华中学',
                address:'中华路'
            }
        },
        methods: {
            showInfo(){
                // 此时this指vc
                alert(this.name)
            }
        },
    }
</script>

/* 配置组件样式 */
<style>
    .name{
        background-color: aqua;
    }
    .address{
        background-color: aqua;
    }
</style>



