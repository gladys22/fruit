<template>
    <div id="app-classify">
        <div class="top-box">
        <div class="shopping-bg">
            <div class="nav-bg"> 
                <a href="#"></a>
                购物车
                <span>编辑</span>
            </div>
            <div class="section-bg">
                <div class="coord">先锋侠需要您的精确坐标</div>
                <div class="time">
                    收货时间 
                    <span>今天30分钟可送达(可预订)</span>
                </div>
                <div class="section">
                    <div class="checkAll">
                        <input class="checkAll-box" type="checkbox">
                        <span class="checkText">自营商品</span>
                    </div>
                    <div class="one-floor">
                        <div class="input_box">
                            <input class="checkAll-box" type="checkbox">
                        </div>

                        <div class="check_detail">
                            <img src="../../images/del/fruits-img12.png" >
                        </div>
                        <div class="check_text">
                            <h6>1SNP 燕窝补水面膜 10片/盒含燕窝精华 双倍补水保湿</h6>
                            <p>¥<span>10.00</span></p>
                            <div class="check_count">
                                <span class="check_add"></span>
                                <input class="count_add" type="tel"  size="4" value="1">
                                <span class="check_minus"></span>
                            </div>
                        </div>
                    </div>
                      <div class="one-floor">
                        <div class="input_box">
                            <input class="checkAll-box" type="checkbox">
                        </div>

                        <div class="check_detail">
                            <img src="../../images/del/fruits-img7.png" >
                        </div>
                        <div class="check_text">
                            <h6>1SNP 新鲜青柠500g/盒新鲜特价</h6>
                            <p>¥<span>10.00</span></p>
                            <div class="check_count">
                                <span class="check_add"></span>
                                <input class="count_add" type="tel"  size="4" value="1">
                                <span class="check_minus"></span>
                            </div>
                        </div>
                    </div>
                    <div class="total">本店总计：¥<sapn>0.00</sapn></div>
                </div>
            </div>
        </div>
</div>
    <div class="pay">
        <label class="pay_checkall">
            <span>
               <input class="checkAll-box pay_input" type="checkbox">
            </span>
            <span class="shop-cart-check1">全选</span>
        </label>
        <span class="scart-total-text2">合计：¥</span>
        <span class="scart-total-text3">0.00</span>
        <a class="scart-total-text4" href="#">去结算</a>
    </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.shopping-bg {
    max-width:640px;
    overflow:hidden;
    margin:0 auto;
}
.nav-bg {
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:44px;
    line-height:44px;
    text-align:center;
    background:#fff;
    border-bottom:1px solid #F6F6F4;
    font-size:16px;
    z-index:22;
    margin:0;
}
.nav-bg a{
    position:absolute;
    top:0;
    left:0;
    width:40px;
    height:44px;
    z-index:22;
    background:url("../../images/arrow-left.png") no-repeat center center;
    background-size:50%;
}
.nav-bg span {
    width:50px;
    line-height:44px;
    position:absolute;
    top:0px;
    right:15px;
    z-index:22;
    font-size:15px;
}
.section-bg {
    width:100%;
    margin-top:45px;
    margin-bottom:96px;
}
.coord {
    width:100%;
    height:40px;
    padding:0 3%;
    margin-bottom:5px;
    font-size:14px;
    line-height:40px;
    background:url("../../images/arrow-right.png") no-repeat 97% center ;
    background-size:6%;
    background-color:#fff;
}
.time {
    width:100%;
    height:40px;
    line-height:40px;
    padding:0 3%;
    font-size:14px;
    background:url("../../images/arrow-right.png") no-repeat 97% center ;
    background-size:6%;
    background-color:#fff;
}
.time span {
    float:right;
    color:#379EDE;
    margin-right:25px;
}
.section {
    width:100%;
    margin-top: 5px;
}
.checkAll {
    width:100%;
    height:35px;
    background:#fff;
    border-bottom:1px solid #F9F9F9;
    padding:0 3%;
}
.checkAll-box {
    width:22px;
    height:22px;
    margin-top:7px;
    position:relative;
     float:left;
}
.checkAll-box::before {
    content:"";
    position:absolute;
    top:0;
    left:0;
    width:22px;
    height:22px;
    background:url("../../images/check3.png") no-repeat center center;
    background-size:100%;
   
}
.checkText {
    margin-left:5px;
    display:block;
    font-size:15px;
    line-height:35px;
    float:left;
}
.one-floor {
    width:100%;
    padding:5px 3%;
    background:#fff;
    border-bottom:1px solid #F9F9F9;
}
.check_detail {
    width:100px;
    height:100px;
    padding:10px 0;
    float:left;
}
.input_box {
    width:30px;
    height:50%;
    float:left;
    margin-top: 33px;
}
.check_detail img{
    width:100%;
}
.check_text {
    height:110px;
    margin-left:140px;
}
.check_text>h6 {
    font-size:15px;
    font-weight:normal;
    color:#333;
    line-height:20px;
    margin-top:10px;
}
.check_text>p {
    width:100%;
    color: #FF9201;
    margin-top: 8px;
    font-size: 18px;
}
.check_count {
width:100%;
}
.check_add {
    width:25px;
    height:25px;
    background:url("../../images/subtract.png") no-repeat center center;
    background-size:100%;
    float:left;
}
.count_add {
    width:20px;
    line-height:25px;
    border:none;
    outline:none;
    font-size:14px;
    padding:0;
    margin:0 4px;
    text-align:center;
    float:left;
    margin-top:-8px;
}
.check_minus{
    width:25px;
    height:25px;
    background:url("../../images/add.png") no-repeat center center;
    background-size:100%;
    float:left;
}
.total {
    width:100%;
    height:40px;
    line-height:40px;
    padding:0 3%;
    background:#fff;
    font-size:14px;
    border-top:1px solid #F9F9F9;
    border-bottom: 1px solid #F9F9F9;
}
.pay {
    width: 100%;
    height: 45px;
    position: fixed;
    bottom: 50px;
    left: 0px;
    background-color: #FFFFFF;
    z-index: 999;
    padding: 0px 3%;
    line-height: 45px;
}
.top-box {
    max-width:640px;
    margin:0 auto;
}
.scart-total-text2 {
    float: left;
    margin: 0 5px 0 7px;
    font-size: 14px;
    color: #A3A3A3;
}
.scart-total-text3 {
    float: left;
    font-size: 16px;
    font-weight: 600;
    color: #FF9201;
}
.scart-total-text4 {
    width: 70px;
    height: 30px;
    line-height: 30px;
    text-align: center;
    background: #FF9201;
    font-size: 14px;
    color: #fff;
    float: right;
    margin-top: 7px;
    border-radius:15px;
}
.pay_checkall {
    float: left;
}
.shop-cart-check1 {
 float: left;
 font-size:16px;
}
.pay_input {
    margin:12px 10px 0 0;
}

</style>