## 文档地址

### 绘制形状

https://developer.mozilla.org/zh-CN/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes

### 使用样式和颜色

fillStyle = color
设置图形的填充颜色。

strokeStyle = color
设置图形轮廓的颜色。

color 可以是表示 CSS 颜色值的字符串，渐变对象或者图案对象。

默认情况下，线条和填充颜色都是黑色（CSS 颜色值 #000000）。

```JS
// 这些 fillStyle 的值均为 '橙色'
ctx.fillStyle = "orange";
ctx.fillStyle = "#FFA500";
ctx.fillStyle = "rgb(255,165,0)";
ctx.fillStyle = "rgba(255,165,0,1)";
```

### 绘制文本

https://developer.mozilla.org/zh-CN/docs/Web/API/Canvas_API/Tutorial/Drawing_text

### 4-使用图片

https://developer.mozilla.org/zh-CN/docs/Web/API/Canvas_API/Tutorial/Using_images

### 5-变形

状态的保存和恢复 Saving and restoring state
在了解变形之前，我先介绍两个在你开始绘制复杂图形时必不可少的方法。

save()
保存画布(canvas)的所有状态
restore()
save 和 restore 方法是用来保存和恢复 canvas 状态的，都没有参数。Canvas 的状态就是当前画面应用的所有样式和变形的一个快照。
Canvas 状态存储在栈中，每当 save()方法被调用后，当前的状态就被推送到栈中保存。一个绘画状态包括：

当前应用的变形（即移动，旋转和缩放，见下）
以及下面这些属性：strokeStyle, fillStyle, globalAlpha, lineWidth, lineCap, lineJoin, miterLimit, lineDashOffset, shadowOffsetX, shadowOffsetY, shadowBlur, shadowColor, globalCompositeOperation, font, textAlign, textBaseline, direction, imageSmoothingEnabled
当前的裁切路径（clipping path），会在下一节介绍
你可以调用任意多次 save 方法。每一次调用 restore 方法，上一个保存的状态就从栈中弹出，所有设定都恢复。

### 6-合成与裁剪

https://developer.mozilla.org/zh-CN/docs/Web/API/Canvas_API/Tutorial/Compositing

### 7-像素操作

https://developer.mozilla.org/zh-CN/docs/Web/API/Canvas_API/Tutorial/Pixel_manipulation_with_canvas
