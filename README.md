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
<table class="main_table" border="0" cellspacing="0" cellpadding="0" width="100%">
<thead>
    <tr class="table_title">
    <td>属性/方法</td>
    <td>说明</td>
    <td>默认值</td>
    </tr>
</thead>
<tbody>
    <tr>
        <td>boxClass</td>
        <td>需要执行动画的元素的class，字符串</td>
        <td>'wow'</td>
    </tr>
    <tr>
        <td>animateClass</td>
        <td>animation.css 动画的class，字符串</td>
        <td>'animated'</td>
    </tr>
    <tr>
        <td>offset</td>
        <td>距离可视区域多少开始执行动画,整数</td>
        <td>0</td>
    </tr>
    <tr>
        <td>mobile</td>
        <td>是否在移动设备上执行动画，布尔值</td>
        <td>true</td>
    </tr>
    <tr>
        <td>live</td>
        <td>异步加载的内容是否有效，布尔值</td>
        <td>true</td>
    </tr>
</tbody>
</table>
