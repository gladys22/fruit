<template>
    <div id="app-home">
         <div class="header-top">
            <div class="top-box1">
                <img src="../../images/scan.png" >
                <span>地址</span>
            </div>
            <div class="top-box2">
                <span>北京石景山</span>
                <span></span>
            </div>
            <div class="top-box3">
                <a href="#">
                    <img src="../../images/search3.png">
                    <span>搜索</span>
                </a>
            </div>
        </div>
        <!-- banner -->
        <mt-swipe >
            <mt-swipe-item v-for="item in list" :key="item.id">
                <img :src="item.img_url">
            </mt-swipe-item>
        </mt-swipe> 
        <!-- nav -->
        <div class="nav">
                <a href="#">
                    <span></span>
                    <p>水果特惠</p>
                </a>
                 <a href="#">
                    <span></span>
                    <p>每日必抢</p>
                </a>
                 <a href="#">
                    <span></span>
                    <p>嗨吃福利</p>
                </a>
                 <a href="#">
                    <span></span>
                    <p>鲜蜂力荐</p>
                </a>
        </div>
        <!-- 1floor -->
       <div class="floor-one">
           <div class="one-bg">
                <span>品牌特卖</span>
                <span></span>
           </div>
           <div class="onedetail-bg">
               <div class="oneimg-bg ">
                    <img src="../../images/del/special-sale-img3.jpg" >
               </div>
               <div class="oneimg-bg">
                    <img src="../../images/del/special-sale-img1.jpg" >
               </div>
              <div class="oneimg-bg">
                    <img src="../../images/del/special-sale-img4.jpg" >
               </div>
           </div>
       </div>
<!--  2floor  -->
<div class="floor-one twofloor-bg">
           <div class="one-bg">
                <span>优选水果</span>
                <span></span>
           </div>
           <div>
               <div class="twoimg-bg ">
                    <img src="../../images/del/optimization-img1.jpg" >
               </div>
               <div class="twoitem-bg">
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img2.png" >
                            <p>新鲜猕猴桃300g</p>
                       </a>
                       <div class="getone">
                           <span> 买一赠一</span>
                        </div>
                       <p>¥22.8 <span>¥31.2</span></p>
                   </div>
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img4.png" >
                            <p>新鲜橙子2斤*1袋</p>
                       </a>
                       <div class="getone"></div>
                       <p>¥18.8 <span>¥24.9</span></p>
                   </div>
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img7.png" >
                            <p>新鲜青柠500/盒</p>
                       </a>
                       <div class="getone"></div>
                       <p>¥10.8 <span>¥12.8</span></p>
                   </div>
               </div>
           </div>
       </div>
    <!--  3floor  -->
   <div class="floor-one twofloor-bg">
           <div class="one-bg">
                <span>酒水饮料</span>
                <span></span>
           </div>
           <div>
               <div class="twoimg-bg ">
                    <img src="../../images/del/optimization-img2.jpg" >
               </div>
               <div class="twoitem-bg">
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img8.png" >
                            <p>可口可乐500g/瓶</p>
                       </a>
                       <div class="getone">
                           <span> 买一赠一</span>
                        </div>
                       <p>¥4.00 <span>¥6.00</span></p>
                   </div>
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img10.png" >
                            <p>RIO鸡尾酒500g/瓶水蜜桃味</p>
                       </a>
                       <div class="getone"></div>
                       <p>¥12.8 <span>¥15.8</span></p>
                   </div>
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img9.png" >
                            <p>百威啤酒400ml/瓶</p>
                       </a>
                       <div class="getone"></div>
                       <p>¥10.8 <span>¥12.8</span></p>
                   </div>
               </div>
           </div>
       </div>
       <!--  4floor  -->
        <div class="floor-one twofloor-bg thirdfloor-bg">
           <div class="one-bg">
                <span>酒水饮料</span>
                <span></span>
           </div>
           <div>
               <div class="twoimg-bg ">
                    <img src="../../images/del/optimization-img3.jpg" >
               </div>
               <div class="twoitem-bg">
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img11.png" >
                            <p>可口可乐500g/瓶</p>
                       </a>
                        <div class="getone">
                           <span> 买一赠一</span>
                        </div>
                       <p>¥4.00 <span>¥6.00</span></p>
                   </div>
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img12.png" >
                            <p>RIO鸡尾酒500g/瓶水蜜桃味</p>
                       </a>
                       <div class="getone"></div>
                       <p>¥12.8 <span>¥15.8</span></p>
                   </div>
                   <div class="twodetail-bg">
                       <a href="#">
                            <img src="../../images/del/fruits-img13.png" >
                            <p>百威啤酒400ml/瓶</p>
                       </a>
                       <div class="getone"></div>
                       <p>¥10.8 <span>¥12.8</span></p>
                   </div>
               </div>
           </div>
       </div>
    </div>
</template>
<script> 
    export default{
        data(){
            return{
                list:[],
                // fid:[],
                // title:[],
                // price:[],
                // or_price:[],
                // img_url:[]
            }
        },
        methods:{
            getImage(){
                this.$http.get("http://127.0.0.1:6600/imagelist").then(result=>{
                this.list=result.body;
            })
            },
            // getfruit(){
            //     this.$http.get("http://127.0.0.1:6600/onedetail").then(result=>{
            //         console.log(result.body)
            //          //this.onefruit=result.body
            //     }
            // )}
        //     getfruit(){
        //         this.axios.get("http://127.0.0.1:6600/onedetail",{
        //             params:{fid:this.fid}
        //         }).then(res=>{
        //             console.log(res.data);
                    
        //         })
        //     }
         },
        created(){
            this.getImage();
            // this.getfruit();
        }
    }
</script>
<style scoped>
p{
    margin:0;
}
.header-top{
        width:100%;
        height:66px;
        position:fixed;
        background:#fff;
        padding:12px 0;
        z-index:22;
        top:0;
        left:0;
        border:1px solid #f1f1f1;
    }
    .top-box1{
        width:17%;
        height:100%;
        float:left;
        text-align:center;
    }
    .top-box1 img{
        width:20px;
        height:20px;
        display:inline-block;
        /* position:relative; */
    }
    .top-box1 span{
        width:100%;
        float:left;
        font-size:12px;
        color:#A8A3A7;
    }
    .top-box2 {
        width:66%;
        height:40px;
        float:left;
        text-align:center;
        line-height:40px;
    }
    .top-box2>span{
         font-size:16px;
        display:inline-block;
    }
    .top-box2>span:nth-child(2){
        width:12px;
        height:12px;
        display:inline-block;
        background:url('../../images/triangle.png') no-repeat center center;
        background-size:100%;
        margin-left:9px;
    }
    .top-box3{
        width:13%;
        height:100%;
        float:left;
        text-align:center;
    }
    .top-box3 a{
        text-decoration:none;
        /* outline:none; */
    }
    .top-box3>a>img{
        width:20px;
        height:20px;
        display:inline-block;
    }
    .top-box3>a>span{
       width:100%;
        float:left;
        font-size:12px;
        color:#A8A3A7;
    }
    /* banner */
    #app-home .mint-swipe {
        width:100%;
        height: 160px;
        margin-top:66px;
    }
  img{
        width:100%;
    }
   /* nav */
    .nav{
        width:100%;
        list-style:none;
        display:flex;
        margin:0;
        padding-bottom:5px;
        background:#fff;
    }
    
    .nav>a{
        width:25%;
        display:inline-block;
        text-align:center;
        font-size:14px;
        margin-top:15px;
    }
    .nav>a>span{
        width:50px;
        height:50px;
        display:inline-block;
        border-radius:50%;
    }
    .nav>a:first-child>span{
        background:url("../../images/trophy.png") no-repeat center center ;
        background-size:26px 26px;
        background-color:#9BCBB5;
    }
    .nav>a>p{
        color: #232326;
        margin-top:2px;
    }
     .nav>a:nth-child(2)>span{
        background:url("../../images/package.png") no-repeat center center ;
        background-size:26px 26px;
        background-color:#E6C3BD;
    }
     .nav>a:nth-child(3)>span{
        background:url("../../images/grass.png") no-repeat center center ;
        background-size:26px 26px;
        background-color:#EED0B8;
    }
     .nav>a:last-child>span{
        background:url("../../images/diamond.png") no-repeat center center ;
        background-size:26px 26px;
        background-color:#8CB2C5;
    }
    /* 1floor */
    .floor-one {
        background:#fff;
        margin-top:5px;
    }
    .one-bg{
        width:100%;
        height:45px;
        text-align:center;
        line-height:45px;
        font-size:16px;
    }
    .one-bg>span:nth-child(2){
        width:18px;
        height:18px;
        background:url("../../images/arrow-right2.png") no-repeat center center;
        background-size:100%;
        display:inline-block;
        vertical-align:middle;
        margin:-3px 0 0 8px;
    }
    .floor-one>.onedetail-bg{
        width:100%;
        padding:0 3% 10px 3%;
        margin:0 auto;
        display:flex;
    }
    .oneimg-bg{
        width:33.3%;
    }
    .oneimg-bg img {
        width:110px;
       
    }
    .floor-one>.onedetail-bg>div:nth-child(2){
        margin-left:5px;
    }
    .floor-one>.onedetail-bg>div:nth-child(3){
        margin-left:5px;
    }
    /* 2floor */
    .floor-one .twoimg-bg {
        width:100%;
        border-radius:50px;
         padding:0px 15px;
    }
    .floor-one .twoimg-bg img{
        width:100%;
         border-radius:50px;
    }
    .twofloor-bg {
         flex-wrap:wrap;
         padding-bottom:10px;
    }
    .twoitem-bg{
        width:100%;
        display:flex;
    }
    .twodetail-bg {
        width:33.3%;
        text-align:center;
        font-size:14px;
    }
   .twodetail-bg img {
    width:75px;
    margin-top:13px;
}
.twodetail-bg>a>p{
    color:#232326;
    font-size:14px;
    margin-top:6px;
    height:40px;
}
.getone{
    height:18px;
}
.getone span{
    height:18px;
    width:62px;
    font-size:12px;
    background:#FF8950;
    line-height:18px;
    color:#fff;
    border-radius:3px;
    padding:0px 7px;
    display:inline-block;
}
.getone p{
    margin-top:5px;
}
.twodetail-bg p:nth-child(3){
    font-size:14px;
    color:#EA4D13;
    margin-top:10px;
}
.twodetail-bg p:nth-child(3)>span{
    color:#979797;
    font-size:12px;
    text-decoration:line-through;
}
.thirdfloor-bg {
    padding-bottom:60px;
}
</style>
