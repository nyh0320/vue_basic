/* 配置组件的模板结构
    template只能有一个根标签，建议用div把所有组件包裹起来
 */
<template>
    <div>
        <School/>
    </div>
</template>

/* 配置组件的数据交互 */
<<script>
    //引入School组件
    import  School from './components/School.vue'

    export default{
        components:{School}
    }
</script>