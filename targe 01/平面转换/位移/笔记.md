## 位移

#### 同时移动水平垂直

语法:transform:translate(水平位移,垂直位移)

-- 可正负,可百分比

#### 移动单个

transform:translateX(水平位移)

transform:translateY(垂直位移)

#### 定位+位移实现居中

定位:父盒子relative,子盒子 absolute   left:50%,top:50%

因为定位是以盒子左上角定位,所以偏移了半个盒子宽和高的距离,此时使用位移挪上去
