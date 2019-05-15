<template>
    <div id="app-classify">
        <div class="personal-top">
                <img src="../../images/599aa36d5e4a4.jpg" >
                <div class="personal-top-box1">
            <span class="personal-top-img1">
                <img src="../../images/20150831135021_JUyLC.jpeg" alt="">
            </span>
            <div class="personal-top-box2">
                <span class="personal-top-text1">青春微凉伴离殇</span>
            </div>
            </div>
            <div class="personal-box1 mbt-05">
          	   <a href="#" class="personal-box2 box3">
          	      <span class="personal-box1-img1"><img src="../../images/personal-center-img1.png" alt=""></span>
          	      <span class="personal-box1-text1">待付款</span>
          	   </a>
          	   <a href="#" class="personal-box2 box3">
          	      <span class="personal-box1-img1"><img src="../../images/personal-center-img2.png" alt=""></span>
          	      <span class="personal-box1-text1">待发货</span>
          	   </a>
          	   <a href="#" class="personal-box2 box3">
          	      <span class="personal-box1-img1"><img src="../../images/personal-center-img3.png" alt=""></span>
          	      <span class="personal-box1-text1">待收货</span>
          	   </a>
          	   <a href="#" class="personal-box2 box3">
          	      <span class="personal-box1-img1"><img src="../../images/personal-center-img4.png" alt=""></span>
          	      <span class="personal-box1-text1">待评价</span>
          	   </a>
          	   <a href="#" class="personal-box2 box3">
          	      <span class="personal-box1-img1"><img src="../../images/personal-center-img5.png" alt=""></span>
          	      <span class="personal-box1-text1">全部订单</span>
          	   </a>
          </div>
        </div>

    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.app-classify {
    max-width: 640px;
    overflow: hidden;
    margin: 0 auto;
}
.personal-top {
    width: 100%;
    /* float: left; */
    position: relative;
    height: 130px;
}
.personal-top img {
    width: 100%;
    /* float: left; */
    height: 130px;
}
.personal-top-img1 {
    width: 70px;
    height: 70px;
    float: left;
    overflow: hidden;
    border: 1px solid #D7D1D1;
    margin-top: 30px;
    border-radius: 50%;
}
.personal-top-box1 {
    width: 100%;
    position: absolute;
    height: 130px;
    top: 0px;
    left: 0px;
    padding: 0px 3%;
}
.personal-top-img1 {
    width: 70px;
    height: 70px;
    border-radius: 50%;
}
.personal-top-img1 img {
   width: 70px;
    height: 70px;
    float: left;
}
.personal-top-box2 {
    display: block;
    margin-left: 80px;
    height: 100px;
    margin-top: 30px;
}
.personal-top-text1 {
    width: 75%;
    float: left;
    height: 25px;
    line-height: 25px;
    white-space: nowrap;
    color: #fff;
    margin-top: 25px;
    font-size:16px;
}
.personal-box1 {
    width: 100%;
    /* float: left; */
    background: #fff;
    padding: 15px 0px;
    margin: 5px 0px;
}
    
</style>