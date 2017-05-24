# flexCase
骰子样式的Flex布局

## 浏览器支持：
![](./img/bg.jpg)

任何容器都可以设置成：display:flex，inline-flex，设置成flex布局之后，子元素的float、clear、vertical-align失效
采用flex布局的元素，称为flex‘容器’，拥有了两个axis（主轴、交叉轴），子元素自动成为容器成员，成为flex item，称为‘项目’，项目默认按照主轴排列。

## 容器属性：

     flex-direction         定义主轴方向
          row | row-reverse | column | column-reverse     
     flex-wrap              项目默认是排在一条轴线上的，wrap定义如何换行
          no-wrap | wrap | wrap-reverse（换行，第一行在下方）
     flex-flow              上面两个属性的简写形式
          flex-direction flex-wrap
     justify-content        主轴内容 在主轴上的对齐方式
          flex-start | flex-end | center | space-between | space-around
     align-items            单一主轴 在交叉轴上的对齐方式
          flex-start | flex-end | center | baseline | stretch（默认，未设置height或为auto，占满高度）
     align-content          多主轴 在交叉轴上的对齐方式
          flex-start | flex-end | center | space-between | space-around | stretch（默认，轴线占满交叉轴高度）

## 项目属性

     order                   项目的排列顺序
     flex-grow               项目的放大比例，默认0【空间富余，不放大】，均为1的话，均分主轴空间
     flex-shrink             项目的缩小比例，默认1【空间不足，就缩小】
     flex-basis              项目占据的主轴空间大小，默认auto【项目本身大小】，浏览器根据该属性计算是否有富余空间
     flex                    上面三个属性的简写形式，默认 0 1 auto
           none | flex-grow flex-shrink flex-basis
     align-self              定义项目与其他项目不一样的对齐方式，覆盖align-items，默认 auto【继承align-items】，没有父元素，为stretch
          auto | flex-start | flex-end | center | baseline | stretch



















     
