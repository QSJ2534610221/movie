<template>
    <div>
            <el-row style="margin-top: 20px">
                <el-col :span="4">
                    <el-radio label="按热度排序"></el-radio>
                </el-col>
                <el-col :span="4">
                    <el-radio label="按时间排序"></el-radio>
                </el-col>
            </el-row>
        <hr/>
            <el-row>
                <el-row v-for="subList in movieList"
                        style="margin-top: 20px">
                    <el-col :span="4">
                        <img v-bind:src="subList[0].imgUrl"/>
                        <div>
                            <span class="title-span" v-on:click="detailpage(subList[0].title)">{{subList[0].title}}</span>
                            &nbsp;&nbsp;
                            <span class="score-span">{{subList[0].score}}</span>
                        </div>
                    </el-col>
                    <el-col :span="4">
                        <img v-bind:src="subList[1].imgUrl"/>
                        <div>
                            <span class="title-span" v-on:click="detailpage(subList[1].title)">{{subList[1].title}}</span>
                            &nbsp;&nbsp;
                            <span class="score-span">{{subList[1].score}}</span>
                        </div>
                    </el-col>
                    <el-col :span="4">
                        <img v-bind:src="subList[2].imgUrl"/>
                        <div>
                            <span class="title-span" v-on:click="detailpage(subList[2].title)">{{subList[2].title}}</span>
                            &nbsp;&nbsp;
                            <span class="score-span">{{subList[2].score}}</span>
                        </div>
                    </el-col>
                    <el-col :span="4">
                        <img v-bind:src="subList[3].imgUrl"/>
                        <div>
                            <span class="title-span" v-on:click="detailpage(subList[3].title)">{{subList[3].title}}</span>
                            &nbsp;&nbsp;
                            <span class="score-span">{{subList[3].score}}</span>
                        </div>
                    </el-col>
                    <el-col :span="4">
                        <img v-bind:src="subList[4].imgUrl"/>
                        <div>
                            <span class="title-span" v-on:click="detailpage(subList[4].title)">{{subList[4].title}}</span>
                            &nbsp;&nbsp;
                            <span class="score-span">{{subList[4].score}}</span>
                        </div>
                    </el-col>
                </el-row>
            </el-row>
    </div>
</template>
<script>
    export default{
        data:function(){
        return{
            movieList:[
               [
                   {title:'小丑',score:9.0,imgUrl:require('../assets/1.jpg')},
                   {title:'海贼王',score:9.9,imgUrl:require('../assets/2.jpg')},
                   {title:'上海堡垒',score:8.0,imgUrl:require('../assets/3.jpg')},
                   {title:'悟空传',score:9.1,imgUrl:require('../assets/4.jpg')},
                   {title:'狂热行动',score:9.9,imgUrl:require('../assets/5.jpg')}
               ] ,
                [
                    {title:'忠犬八公',score:9.1,imgUrl:require('../assets/6.jpg')},
                    {title:'我不是药神',score:9.2,imgUrl:require('../assets/7.jpg')},
                    {title:'速度与激情',score:9.1,imgUrl:require('../assets/8.jpg')},
                    {title:'余罪',score:9.3,imgUrl:require('../assets/9.jpg')},
                    {title:'钢铁侠',score:9.1,imgUrl:require('../assets/10.jpg')}
                ]
            ]
        }
    },
        methods:{
            detailpage:function(title){
                this.$router.push({name:"movie",params:{title:title}});

            }
        }
    }
</script>
<style scoped>
    img{
        width:160px;
        height:240px;
    }
    .title-span{
        cursor:pointer;
        coler:#33A1D7;
    }
    .score-span{
        color: #ffb400;

    }
</style>