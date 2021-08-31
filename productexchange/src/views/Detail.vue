<template>
  <div class="center_con clearfix">
		<div class="main_menu fl"><img src="https://m.media-amazon.com/images/I/71seiDsvWqL._AC_SX466_.jpg"></div>
		<div class="goods_detail_list">
			<h3>Apple MacBook Air</h3>
			<p>Apple MacBook Air with Apple M1 Chip (13-inch, 8GB RAM, 256GB SSD Storage) - Silver (Latest Model)</p>
            <p>
                <span>Seller:  </span><span>Robert</span><br />
                <span>Credit:  </span><span>95</span>
            </p>
			<div class="prize_bar">
				<div class="show_prize fl">$<em>1349</em></div>
			</div>
			<div class="operate_btn">
				<a href="" class="buy_btn">buy now</a>
			</div>
		</div>
	</div>
</template>

<script>
export default {

}
</script>

<style>

.submena{
    width: 100%;
    height: 30px;
    margin: 0 auto;
    /*background:yellow;*/
}
.submena a{
    color:#37ab40;
    line-height: 30px;
}

.center_con{
	width:100%;
  height:100;
	margin: 0 auto;
	/*background: yellow;*/
}
.center_con .main_menu{
	width:100%;
  height:100%;
  overflow:hidden;
}

.goods_detail_list h3{
    font-size:24px;
    line-height:24px;
    color:rgb(212, 56, 56);
    font-weight:normal;
    margin: 0 auto;
}
.goods_detail_list p{
    color:#666;
    line-height:40px;
}
.prize_bar{
    height:72px;
    background-color:#fff5f5;
    line-height:72px;
}
.prize_bar .show_prize{
    font-size:20px;
    color:#ff3e3e;
    padding-left:20px
}
.operate_btn{
    height:40px;
    margin-top:35px;
    font-size:0;
    position:relative;
}
.operate_btn .buy_btn{
    display:inline-block;
    width:178px;
    height:38px;
    border:1px solid #c40000;
    font-size:14px;
    color:#c40000;
    line-height:38px;
    text-align:center;
    background-color:#ffeded;
}
</style>