<template>
    <div>
        <el-row><h1 style="margin-top: 30px;margin-right: 1200px">豆瓣电影排行榜</h1>
            <div style="margin-right: 1260px"><h3 style="color: #058304">豆瓣新片榜· · · · · ·</h3></div>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
            <img src="../assets/1.jpg" style="width: 150px; height: 200px">
        </el-col>
                <el-col :span="8" style="text-align: justify">
               <div style="margin-top: 20px; color: #466ba9">小丑/小丑起源电影：罗密欧/Romeo</div>
                    <div style="margin-top: 20px;color: #5d5d5d">2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 / 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普...
                    </div>
                    <div style="margin-top: 25px;">
                        <el-rate
                                v-model="value1"
                                disabled
                                text-color="#ff9900"
                                text-template="{value}">
                        </el-rate>
                    </div>
                    <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">8.8</a>  &nbsp;(123358人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/10.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">钢铁侠/lron Man</div>
                <div style="margin-top: 20px;color: #5d5d5d">美国 / 动作 / 冒险 / 科幻 / 惊悚 / 铁甲奇侠(港) / 钢铁人(台) / 126分钟
                    乔恩·费儒 / 小罗伯特·唐尼 / 泰伦斯·霍华德 / 格温妮斯·帕特洛 / 杰夫·布里吉斯 / 莱丝莉·比伯 / 肖恩·托布 / 保罗·贝坦尼
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value2"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">8.7</a>  &nbsp;(2354563人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/7.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">我不是药神（2018）</div>
                <div style="margin-top: 20px;color: #5d5d5d">中国大陆 / 剧情 / 喜剧 / 中国药神 / 印度药神 / 117分钟
                    文牧野 / 徐峥 / 王传君 / 周一围 / 谭卓 / 章宇 / 杨新鸣 / 王佳佳 / 王砚辉
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value3"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">8.9</a>  &nbsp;(45358人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/6.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">忠犬八公（美国）</div>
                <div style="margin-top: 20px;color: #5d5d5d">美国 / 英国 / 剧情 / 忠犬小八(台) / 秋田犬八千(港) / 93分钟
                    拉斯·霍尔斯道姆 / 理查·基尔 / 萨拉·罗默尔 / 琼·艾伦 / 罗比·萨布莱特 / 艾瑞克·阿瓦利 / 田川洋行 / 杰森·亚历山大 /
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value4"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">9.0</a>  &nbsp;(3358人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/5.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">狂热行动（日本）</div>
                <div style="margin-top: 20px;color: #5d5d5d">日本 / 动画 / 冒险 / 航海王：夺宝争霸战(台) / 海贼王：狂热行动 / 101分钟
                    大塚隆史 / 田中真弓 / 冈村明美 / 中井和哉 / 山口胜平 / 平田广明 / 大谷育江 / 山口由里子 / 矢尾一树
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value5"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">9.2</a>  &nbsp;(6358人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/8.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">速度与激情（美国）</div>
                <div style="margin-top: 20px;color: #5d5d5d">美国 / 动作 / 犯罪 / 霍布斯与肖 / 速度与激情外传 / 137分钟
                    大卫·雷奇 / 道恩·强森 / 杰森·斯坦森 / 伊德里斯·艾尔巴 / 凡妮莎·柯比 / 艾莎·冈萨雷斯 / 海伦·米伦 / 瑞恩·雷诺兹 / 凯
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value6"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">9.1</a>  &nbsp;(8358人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/3.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">上海堡垒（内地）</div>
                <div style="margin-top: 20px;color: #5d5d5d">中国大陆 / 爱情 / 战争 / 科幻 / Shanghai Fortress / 107分钟
                    滕华涛 / 鹿晗 / 舒淇 / 石凉 / 高以翔 / 王宫良 / 王森 / 孙嘉灵
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value7"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">8.1</a>  &nbsp;(23358人评价)</div>
            </el-col>
        </el-row>
        <hr style="width: 800px;margin-left: 0"/>
        <el-row>
            <el-col :span="4">
                <img src="../assets/9.jpg" style="width: 150px; height: 200px">
            </el-col>
            <el-col :span="8" style="text-align: justify">
                <div style="margin-top: 20px; color: #466ba9">余罪（内地）</div>
                <div style="margin-top: 20px;color: #5d5d5d">《余罪》是爱奇艺、新丽传媒、天神娱乐联合出品的悬疑犯罪
                    网剧，由张睿执导，沈嵘、张仕栋等担任编剧，张一山、常戎、吴优、张锦程等主演
                </div>
                <div style="margin-top: 25px;">
                    <el-rate
                            v-model="value8"
                            disabled
                            text-color="#ff9900"
                            text-template="{value}">
                    </el-rate>
                </div>
                <div style="margin-top: -20px;margin-left: 120px"><a style="color: #b88b1f">9.0</a>  &nbsp;(223358人评价)</div>
            </el-col>
        </el-row>
    </div>
</template>
<script>
    import ElRow from "element-ui/packages/row/src/row";
    export default {
        components: {ElRow},
        data() {
            return {
                value1:4.0,
                value2:2.5,
                value3:4.5,
                value4:4.0,
                value5:5.0,
                value6:4.5,
                value7:2.0,
                value8:4.5
            }
        }
    }
</script>
