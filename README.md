# wow.js
使用方法
1、引入文件

<link rel="stylesheet" href="css/animate.min.css">
2、HTML

<div class="wow slideInLeft"></div>
<div class="wow slideInRight"></div>
可以加入 data-wow-duration（动画持续时间）和 data-wow-delay（动画延迟时间）属性，如：

<div class="wow slideInLeft" data-wow-duration="2s" data-wow-delay="5s"></div>
<div class="wow slideInRight" data-wow-offset="10"  data-wow-iteration="10"></div>
3、JavaScript

new WOW().init();
如果需要自定义配置，可如下使用：

var wow = new WOW({
    boxClass: 'wow',
    animateClass: 'animated',
    offset: 0,
    mobile: true,
    live: true
});
wow.init();

选项配置
