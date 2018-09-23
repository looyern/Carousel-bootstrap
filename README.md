# Carousel-bootstrap<br>
```
<div class="container">
        <h2 class="text-center">轮播展示</h2>
        <!--data-ride="carousel"激活轮播，即让图片自动播放-->
        <div id="myCarousel" class="carousel slide text-center" data-ride="carousel">
            <!--控制器,即轮播图下方的小圆点-->
            <ol class="carousel-indicators">
                <!--data-target="#myCarousel"用于点击圆点切换图片-->
                <li data-target="#myCarousel" data-slide-to="2" class="active"></li>
                <li data-target="#myCarousel" data-slide-to="4"></li>
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
