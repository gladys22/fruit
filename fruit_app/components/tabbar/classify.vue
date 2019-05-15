<template>
    <div id="app-classify">
        <!--tou-->
    <div class="top-bg">
        <div class="topitem-bg">
            <span>派送至：北京石景山</span>
            <span></span>
        </div>
        <div class="search-bg">
            <span>
                <img src="../../images/search3.png" >
            </span>
        </div>
    </div>
<!--侧栏-->
<div class="bigbox">
    <!--左-->
    <div class="side_left">
        <div class="side-perch"></div>
        <span class="side-option">热销新品</span>
        <span class="side-option">优选水果</span>
        <span class="side-option">卤味熟食</span>
        <span class="side-option">牛奶面包</span>
        <span class="side-option">热饮</span>
        <span class="side-option">冰淇淋</span>
        <span class="side-option">饮料酒水</span>
        <span class="side-option">休闲零食</span>
        <span class="side-option">方便速食</span>
        <span class="side-option">数码家电</span>
        <span class="side-option">环球美食</span>
        <span class="side-option">运动户外</span>
    </div>
      <!--右-->
    <div class="side-right">
        <div class="side-perch2"></div>
        <div class="top-option">
            <span class="left_tab">综合排序</span>
            <span class="middle_tab">
                按价格
            <i class="img1"></i>
            <i class="img2 img3"></i>
            </span>
            <span class="right_tab">分类</span>
        </div>
        <!--下拉菜单-隐藏-->
        <div class="rtop-list">
            <span class="rtop-item col_active">全部分类</span>
            <span class="rtop-item">进口水果</span>
            <span class="rtop-item">国产水果</span>
            <span class="rtop-item">柑橘橙柚</span>
            <span class="rtop-item">苹果/梨</span>
            <span class="rtop-item">桃杏梅枣</span>
        </div>
        <!--商品列表-->
        <div class="rbottm-list" v-for="tmp of list" :key="tmp.fid">
            <a class="img-box" href="#">
                <img :src="'http://127.0.0.1:6600/'+tmp.img_url" >
            </a>
            <div class="right-text">
                <a class="r_title" href="">{{tmp.title}}</a>
                <span class="r_price">￥10.8</span>
                <div class="shopcart-box">
                    <span class="leftcart-box"></span>
                    <input class="middlecart-box" type="tel" size="4" value="0" id="tb_count">
                    <span class="rightcart-box"></span>
                </div>
            </div>
            
        </div>
        <div class="rb-item"></div>
        <div class="rb-item"></div>
        <div class="rb-item"></div>
        <div class="rb-item"></div>
        <div class="rb-item"></div>
        <div class="rb-item"></div>
        <div class="rb-item"></div>
    </div>
</div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            list:[],
        }
    },
   created(){
        this.getList();
    },
    methods:{
        getList(){
            this.axios.get("http://127.0.0.1:6600/List").then(res=>{
               this.list=res.data;
            })
        }
    }
}
</script>
<style scoped>
/*tou*/
.top-bg {
    width:100%;
    height:45px;
    background:#fff;
    position:fixed;
    top:0;
    left:0;
    z-index:22;
    border-bottom:1px solid #f1f1f1;
}
.topitem-bg {
    width:100%;
    height:45px;
    line-height:45px;
    text-align:center;
}
.topitem-bg>span:first-child{
    font-size:16px;
    display:inline-block;
}
.topitem-bg>span:nth-child(2){
    width:12px;
    height:12px;
    background:url("../../images/triangle.png") no-repeat center center;
    background-size:100%;
    display:inline-block;
    margin-left:10px;
}
.search-bg {
    width:17%;
    height:100%;
    position:absolute;
    top:13px;
    right:0;
    text-align:center;
}
.search-bg span {
    width:20px;
    height:20px;
    display:inline-block;
    
}
.search-bg span img{
    width:100%;
}
.bigbox{
    width:100%;
    height:100%;
    position:fixed;
    top:0;
    left:0;
    z-index:1;
    background:#fff;
}
.side_left{
    width:30%;
    height:100%;
    overflow-x:hidden;
    overflow-y:auto;
    float:left;
    border-right:1px solid #F4F4F4;
}
.side-perch {
    width:100%;
    height:45px;
}
.side-option {
    width:100%;
    height:40px;
    line-height:40px;
    font-size:14px;
    display:block;
    text-align:center;
    border-bottom:1px solid #EFEAEE;
}
/*右*/
.side-right{
    width:70%;
    height:100%;
    float:right;
    /* overflow-x:hidden;
    overflow-y:auto; */
}
.side-perch2 {
    width:100%;
    height:45px;
}
.top-option {
    width:100%;
    height:40px;
    border-bottom:1px solid #EFEAEE;
}
.left_tab {
    width:33.3%;
    height:40px;
    line-height:40px;
    text-align:center;
    font-size:12px;
    float:left;
}
.middle_tab {
    width:33.3%;
    height:40px;
    line-height:40px;
    text-align:center;
    font-size:12px;
    float:left;
}
.img1{
    width:15px;
    height:15px;
    display:inline-block;
    background:url('../../images/sort1.png') no-repeat center center;
    background-size:100%;
    vertical-align:middle;
    margin-top:-3px;
}
.img2 {
    width:15px;
    height:15px;
    display:inline-block;
    background:url('../../images/sort2.png') no-repeat center center;
    background-size:100%;
    vertical-align:middle;
    margin-top:-3px;
    display:none;
}
.img3 {
    width:15px;
    height:15px;
    display:inline-block;
    background:url('../../images/sort3.png') no-repeat center center;
    background-size:100%;
    vertical-align:middle;
    margin-top:-3px;
    display:none;
}
.right_tab {
    width:33.3%;
    height:40px;
    font-size:12px;
    line-height:40px;
    text-align:center;
    display:inline-block;
}
.rtop-list {
    width:70%;
    border-bottom:1px solid #EFEAEE;
    position:fixed;
    top:87px;
    right:0;
    padding-top:10px;
    display:none;
}

.rtop-item {
    width:30%;
    height:22px;
    font-size:12px;
    border:1px solid #EFEFEF;
    border-radius:3px;
    line-height:22px;
    text-align:center;
    margin-bottom:10px;
    /* display:inline-block; */
    float:left;
    margin-left:2%;
}
.col_active{
    color:#FF9201;
    border-color:#FF9201;
}
.rbottm-list {
    width:100%;
    height:80px;
    border-bottom:1px solid #EFEFEF;
    padding-right:5px;
}
.img-box {
    width:80px;
    height:80px;
    float:left;
    /* display:inline-block; */
    text-align:center;
    padding:10px;
    box-sizing:border-box;
}
.img-box>img{
    width:100%;
}
.right-text {
    margin-left: 80px;
    height: 75px;
    margin-top: 5px;
}
.r_title {
    width:100%;
    float: left;
    font-size:14px;
    color:#232326;
}
.r_price {
    float:left;
    font-size:14px;
    color:#FF9201;
    line-height:30px;
    margin-top:5px;
}
.shopcart-box {
    float:right;
    height:5px;
    margin-right:5px;                                                                                                          
}
.leftcart-box {
    float: left;
    width:20px;
    height:20px;
    background:url("../../images/subtract.png") no-repeat center center;
    background-size:100%;
    margin-top:10px;
}
.middlecart-box {
    width:25px;
    outline:none;
    font-size:14px;
    float:left;
    border:none;
    text-align:center;
    padding:0;
    height:20px;
    margin-top:10px;
}
.rightcart-box {
    float:left;
    width:20px;
    height:20px;
    background:url("../../images/add.png") no-repeat center center;
    background-size:100%;
    margin-top:10px;
}
</style>

