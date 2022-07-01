# 旋转

语法 :transform: rotate(1000deg角度);

注意点:**旋转必须要有过渡**,不然不生效

### 转换旋转原点

默认是中心点旋转,我们可以修改以哪个点旋转


参数 left right top bottom center

transform-origin: right   bottom ;


### 多重转换

transform: translateX(600px) rotate(1000deg);

先平移在旋转,顺序不能变

如果先旋转,就会改变坐标轴,然后平移,就会出现绕一个大圈的效果
