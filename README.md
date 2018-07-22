## canvas 坐标
![canvas](./static/canvas1.png)<br/><br/>
 canvas的坐标横轴为x轴(正方向朝右),纵轴为y轴(正方向朝下)
 ## 程序简单步骤
![canvas](./static/canvas2.png)<br/><br/>
1. 获取canvas: `var canvas = doucment.getElementById('webgl')`
2. 获取上下文: `var gl = getWebGLContext(canvas)`
3. 设置背景色: `gl.clearColor(0.0, 0.0, 0.0, 1.0)`
4. 清空canvas: `gl.clear(gl.COLOR_BUFFER_BIT)`
