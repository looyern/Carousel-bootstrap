# Carousel-bootstrap<br>
```
<div class="container">
   <h2 class="text-center">轮播展示</h2>
   <div id="myCarousel" class="carousel slide text-center" data-ride="carousel">
      <ol class="carousel-indicators">
         <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
         <li data-target="#myCarousel" data-slide-to="1"></li>
         <li data-target="#myCarousel" data-slide-to="2"></li>                
      </ol>
      <!--轮播项目-->
      <div class="carousel-inner">
          <div class="item active">
               <img src="https://static1.bcjiaoyu.com/f49febe723ba79c384a71a62e3571f2d_o.png-1200x800" alt="First">
          </div>
          <div class="item">
               <img src="https://static1.bcjiaoyu.com/519a8173d4933b4344c667cd389fd6ae_j.png-1200x800" alt="Second">
          </div>
          <div class="item">
               <img src="https://static1.bcjiaoyu.com/770b3bd613dacfbeb225474068497adc_d.png-1200x800" alt="Third">
          </div>                                
      </div>
      <!--轮播导航-->
          <a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">
               <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
          </a>
          <a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">
               <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
          </a>
      </div>
</div>
```
以上是简易轮播图的代码<br>
知识点详解：<br> 
```
<div id="myCarousel" class="carousel slide text-center" data-ride="carousel">
      <ol class="carousel-indicators">
         <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
         <li data-target="#myCarousel" data-slide-to="1"></li>
         <li data-target="#myCarousel" data-slide-to="2"></li>                
      </ol>
```
   *  有序列表的作用是用来添加轮播图下方的小圆点;
   *  `data-ride="carousel"`用于激活轮播，让图片实现自动播放;
   *  `data-target`指向`data-ride`所在元素的id;
   *  `data-target="#myCarousel" ` 点击圆点可以切换图片;
   *  `<ol class="carousel-indicators">中的class="carousel-indicators"`用于轮播圆点的设置，使之以圆点的形式置于图片下方
   *  `data-slide-to` 用于切换至相对应的图片,`data-slide-to="0"`数字代表的是图片的索引值，索引从0开始;
         *图片的索引与按钮是一一对应的：第一个按钮对应的是第一张图片（索引是0），因此是`data-slide-to="0"`
```
<div class="carousel-inner">
    <div class="item active">
         <img src="https://static1.bcjiaoyu.com/f49febe723ba79c384a71a62e3571f2d_o.png-1200x800" alt="First">
    </div>
    <div class="item">
         <img src="https://static1.bcjiaoyu.com/519a8173d4933b4344c667cd389fd6ae_j.png-1200x800" alt="Second">
    </div>
    <div class="item">
         <img src="https://static1.bcjiaoyu.com/770b3bd613dacfbeb225474068497adc_d.png-1200x800" alt="Third">
    </div>                                
</div> 
```
   *  `<div class="carousel-inner">`是包裹着整个轮播项目的盒子，必须设置；
   *  `<div class="item">`每个 .item 包裹的都是一个轮播项目；
   *  `<div class="carousel-caption">标题 1</div>`若想为轮播图设置一个标题，则需要在 .item 中插入该代码，标题会会自动对齐并格式化（位于轮播圆点上方）。
```
      </div>
          <a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">
               <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
          </a>
          <a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">
               <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
          </a>
      </div>
```
   *  用<a>标签的超链接实现点击切换，同样链接 href 指向启用轮播的元素(即`data-ride`所在元素的id)；
   *  `class="left carousel-control"`.carousel-control用于显示轮播箭头并调用点击切换图片的功能；
      *  .left指定轮播箭头位于轮播项的左边。
   *  `data-slide="prev"`表示切换到上一个轮播项，next则是切换至下一个轮播项；
   *  `aria-hidden="true"` .aria-* 用于支持读屏设备的，方便残障人士使用。


