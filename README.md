# Carousel-bootstrap<br>
```
<div class="container">
        <h2 class="text-center">轮播展示</h2>
        <div id="myCarousel" class="carousel slide text-center" data-ride="carousel">
            <!--控制器,即轮播图下方的小圆点-->
            <ol class="carousel-indicators">
                <!--data-target="#myCarousel"用于点击圆点切换图片-->
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
其中包含的知识点：<br>1.激活轮播，即让图片实现自动播放：
```
data-ride="carousel"
```
2.
```
<ol class="carousel-indicators">
   <!--data-target="#myCarousel"用于点击圆点切换图片-->
   <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
   <li data-target="#myCarousel" data-slide-to="1"></li>
   <li data-target="#myCarousel" data-slide-to="2"></li>                
</ol>
```
                有序列表的作用是用来添加轮播图下方的小圆点;
                data-target="#myCarousel"  点击圆点可以切换图片；
                data-slide-to 用于切换至相对应的图片。
