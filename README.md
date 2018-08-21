1.精灵图的 background-size 设置？
  移动端

2.ul里面的font-size:0 的作用？
更好的还原设计稿，在父元素很有必要设置font-size:0，避免莫名其妙的间距。

3.弹性盒模型  父 display:flex  子 flex:1; 

body {
    direction: rtl;
}
 
.flex-container {
    display: -webkit-flex;
    display: flex;
    width: 400px;
    height: 250px;
    background-color: lightgrey;
}
 
.flex-item {
    background-color: cornflowerblue;
    width: 100px;
    height: 100px;
    margin: 10px;
}
4.浮动元素的作用
在网页布局中，块级元素在一行显示就使用浮动 float:left;
如果只是希望一个行内元素有宽度或者高度（进行模式转换），就使用display  display:inlineblock/block;

使用场景：1为了实现图片和文字环绕效果，而设计了浮动该属性。2网页布局块级元素在一行显示3在网页布局中制作导航栏


5.flex布局 只是用局部具有伸缩性的布局
伸缩容器：display:flex;
伸缩项目：伸缩容器的直接子元素；

flex属性定义的是伸缩项目所占的伸缩容器剩余空间的比例；

子元素垂直水平居中 --弹性模式
 .parent{
     display:flex;
     justify-content:center;
     align-items:center;
 }

 设置主轴方向：flex-direction 四个 row column
 设置伸缩项目在主轴方向的对齐方式：justify-content:flex-start end center space-between  around

 伸缩项目是否换行 flex-wrap nowrap wrap
    换行之后的对齐方式 align-content 跟 justify-content
    不换行的对齐方式  align-item:flex-start end center stretch baseline