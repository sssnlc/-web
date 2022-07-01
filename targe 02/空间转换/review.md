# 空间转换

## 空间平移

```css
transform: translate3d(100px,100px,200px);
```

空间上就是比之前平面平移多了一个z轴

**你想一下一个x和y轴，那么z轴就是垂直于屏幕的，所以我们看不出这种效果，z轴为正，就算往外，视觉效果是变大，往内呢z轴为负，就是变小，可以理解为近大远小**

在我们正常的视角情况下，我们是看不到z轴的变化，那么css给我们提供了一个属性

perspective: 1000px（一般在800~1200，需要添加给父级，也就是需要空间平移的盒子的父级元素）;，它能够是我们看到改变z的效果



**perspective实现了透视**

原理：

[黑马程序员web前端进阶教程，前端html5+css3+移动端项目实战（含华为新闻，b站移动端等）_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1xq4y1q7jZ?p=31&vd_source=e415db0e6ae35ffef3a5f48b39912ccb)


## 空间旋转：


```css
    transform: rotateX(360deg);

    transform: rotateY(360deg);

    transform: rotateZ(360deg)
```

x就是绕水平x转

y就是绕y转

z就是绕中心轴（跟之前得水平旋转一样）

记住也必须在父盒子设置属性 perspective: 1000px
