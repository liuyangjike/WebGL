# ch2
## 坐标图
 >![canvas](./static/canvas1.png)<br/>
 >canvas的坐标横轴为x轴(正方向朝右),纵轴为y轴(正方向朝下)<br/>
![canvas](./static/canvas3.png)<br/>
 >webgl的右手坐标<br/>
![canvas](./static/canvas4.png)<br/>
 >对应坐标<br/>
 ## 绘图简单步骤
![canvas](./static/canvas2.png)<br/>
1. 获取canvas: `var canvas = doucment.getElementById('webgl')`
2. 获取上下文: `var gl = getWebGLContext(canvas)`
3. 初始化着色器  `initShader(gl, VSHADER_SOURCE, FSHADER_SOURCE)`
4. 设置背景色: `gl.clearColor(0.0, 0.0, 0.0, 1.0)`
5. 清空canvas: `gl.clear(gl.COLOR_BUFFER_BIT)`
6. 绘图: `gl.drawArrays(gl.POINTS, 0, 1)`
## 要点
1. WebGL程序包括运行在浏览器中的Javascript和运行在WebGL系统的着色器程序俩个部分
2. vec4 四个浮点数 组成的矢量(也称为齐次坐标是四维的,通常把最后一个变量设置为1.0代表三维)
3. 顶点着色器两个内置变量: `gl_Position, gl_PointSize`
4. 片元着色器内置变量:  `gl_FragColor`
