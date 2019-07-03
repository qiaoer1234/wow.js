# wow.js
使用方法

<p>1、引入文件</p>
<pre><code class="html">&lt;link rel="stylesheet" href="css/animate.min.css"&gt;
</code></pre>
<p>2、HTML</p>
<pre><code class="html">&lt;div class="wow slideInLeft"&gt;&lt;/div&gt;
&lt;div class="wow slideInRight"&gt;&lt;/div&gt;
</code></pre>
<p>可以加入 data-wow-duration（动画持续时间）和 data-wow-delay（动画延迟时间）属性，如：</p>
<pre><code class="html">&lt;div class="wow slideInLeft" data-wow-duration="2s" data-wow-delay="5s"&gt;&lt;/div&gt;
&lt;div class="wow slideInRight" data-wow-offset="10"  data-wow-iteration="10"&gt;&lt;/div&gt;
</code></pre>
<p>3、JavaScript</p>
<pre><code class="js">new WOW().init();
</code></pre>

<p>如果需要自定义配置，可如下使用：</p>
<pre><code class="js">var wow = new WOW({
    boxClass: 'wow',
    animateClass: 'animated',
    offset: 0,
    mobile: true,
    live: true
});
wow.init();
</code></pre>

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
