<template>
  <div>
    <mt-swipe :auto="2000">
      <mt-swipe-item v-for="(item,index) in list" :key="index"><img :src="item" alt=""></mt-swipe-item>
    </mt-swipe>
    <ul class="mui-table-view mui-grid-view mui-grid-9">
		            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3"><a href="#">
		                    <span class="mui-icon mui-icon-home"></span>
		                    <div class="mui-media-body">新闻资讯</div></a></li>
		            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3"><a href="#">
		                    <span class="mui-icon mui-icon-email"><span class="mui-badge">5</span></span>
		                    <div class="mui-media-body">图片分享</div></a></li>
		            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3"><a href="#">
		                    <span class="mui-icon mui-icon-chatbubble"></span>
		                    <div class="mui-media-body">商品购买</div></a></li>
		            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3"><a href="#">
		                    <span class="mui-icon mui-icon-location"></span>
		                    <div class="mui-media-body">留言反馈</div></a></li>
		            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3"><a href="#">
		                    <span class="mui-icon mui-icon-search"></span>
		                    <div class="mui-media-body">视频专区</div></a></li>
		            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3"><a href="#">
		                    <span class="mui-icon mui-icon-phone"></span>
		                    <div class="mui-media-body">联系我们</div></a></li>
		        </ul>
  </div>
</template>
<script>
export default {
    data(){
        return{
            list:[
              "http://pic37.nipic.com/20140113/8800276_184927469000_2.png",
              "http://pic31.nipic.com/20130801/11604791_100539834000_2.jpg",
              "http://img.redocn.com/sheji/20141219/zhongguofengdaodeliyizhanbanzhijing_3744115.jpg"
            ]
        }
    }
    // created(){
    //    this.getlunbotu();
    // },
    // methods:{
    //     getlunbotu(){
    //         this.$http.get("http://vue.studyit.io/api/getlunbo").then(result=>{
    //              console.log(result.body);
    //         });
    //     }
    // }
};
</script>
<style  scoped>
  .mint-swipe{
    height: 200px;
   }
 .mint-swipe-item img{
        width: 100%;
        height: 100%;
       }
.mui-grid-view.mui-grid-9{
  background: #fff;
  border: none;
}
.mui-grid-view.mui-grid-9 .mui-table-view-cell{
  border: 0;
}
.mui-grid-view.mui-grid-9 .mui-media-body{
  font-size: 13px;
}
</style>
