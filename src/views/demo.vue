<template>
    <div>
        <h1>{{content}}</h1>
        请输入：<input type="text" v-model="content">
        <el-button type="warning" round>按钮</el-button>
    </div>
</template>
<script>
    //noinspection JSAnnotator
    export default {
        data:function () {
            return{
                content:""
            }

        }
    }
</script>
<style scoped>
    h1{
        color: cornflowerblue;
    }
</style>