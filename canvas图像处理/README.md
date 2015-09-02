###1 `drawImage`
> 在 canvas 上绘制图片

语法：
```
ctx.drawImage(img, dx, dy);
ctx.drawImage(img, dx, dy, dWidth, dHeight);
ctx.drawImage(img, sx, sy, sWidth, sHeight, dx, dy, dWidth, dHeight );
```

参数值：


| 参数 | 描述 |
|--------|--------|
|    img    |   绘制到上下文的元素.HTMLImageElement，HTMLVideoElement，或者 HTMLCanvasElement。     |
|    dx    |   源图像的左上角在目标canvas上 X 轴的位置。     |
|    dy    |   源图像的左上角在目标canvas上 Y 轴的位置。     |
|    dWidth    |   在目标canvas上绘制图像的宽度。允许对绘制的图像进行缩放。     |
|    dHeight    |   在目标canvas上绘制图像的高度。允许对绘制的图像进行缩放。     |
|    sx    |   需要绘制到目标上下文中的，源图像的矩形选择框的左上角 X 坐标。     |
|    sy    |  需要绘制到目标上下文中的，源图像的矩形选择框的左上角 Y 坐标。     |
|    sWidth    |  需要绘制到目标上下文中的，源图像的矩形选择框的宽度。     |
|    sHeight    |  需要绘制到目标上下文中的，源图像的矩形选择框的高度。     |
![canvas drawImage](pic/Canvas_drawimage.jpg)

###2 `clearRect`
> 在 canvas 上绘制图片

语法：
```
ctx.clearRect(x, y, width, height);
```

参数值：


| 参数 | 描述 |
|--------|--------|
|    x    |   要清除的矩形左上角的 x 坐标     |
|    y    |   要清除的矩形左上角的 y 坐标     |
|    width    |   要清除的矩形的宽度     |
|    height    |   要清除的矩形的高度     |

###3. 离屏canvas
>离屏canvas经常用来存放临时性的图像信息

使离屏canvas遵循的四个步骤：
1. 创建用做离屏canvas的元素
2. 设置离屏canvas的宽度与高度
3. 在离屏canvas之中进行绘制
4. 将离屏canvas的全部或者一部分内容复制到正在显示的canvas之中
