# 基础补充

## 如何进行精灵抠图

-- 首页一个div,设置背景图

```css
  background-image: url('./img/bg.png');
```

-- 然后使用抠图

```css
background-position:宽 高
```

## 浮动的注意点

当你使用浮动,一个div里一个ul和多个li

这个时候你想要把li浮动到div里,此时呢div又只需要这么大,有li被由于空间不足被挤下来

**解决**:1.当然可以调大div的空间

    2.我们可以设置ul的空间大小


## 盒子模型的注意点:

发现使用盒子模型的时候magin啊会改变盒子的尺寸就会影响布局,所以还是用定位好


# 无缝走马灯

### 如何实现无缝呢?

例如你总共8张图片,而展示区域为2张,那么只需要将头两个给复制到最后,此时你有10张图,这样就会有一种无缝的效果

### 实现走马灯

一个大的ul在一个小的div里,设置个动画移动这个ul,溢出div隐藏就可以了


# 设置网页背景图

首先我们想一个背景刚好铺满整个屏幕

这样设置

-- 默认的话,浏览器html的高度是为0px的,我们想让图片沾满屏幕,就要body沾满,body又需要html占满,所以必须设置html和body的高度

-- no -repeat :不平铺(默认如果一个图片没铺满就会在下面继续铺)

-- center:背景居中

-- 缩放背景图:background-size: cover;

    -- cover图片完全覆盖盒子,但是可能会导致图片不全

    -- contain保证图片的等比例缩放,当宽或高跟盒子尺寸相等,图片就不会缩放了

```css
html {
  height: 100%;
}

body {
  height: 100%;
  width: 100%;
  background: url('./img/f1_1.jpg') no-repeat center;

  /* 缩放背景图 */
  /* contain保证图片的等比例缩放,
  当宽或高跟盒子尺寸相等,图片就不会缩放了 */
  /* background-size: contain; */
  /* cover图片完全覆盖盒子,但是可能会导致图片不全 */
  background-size: cover;
}

```
