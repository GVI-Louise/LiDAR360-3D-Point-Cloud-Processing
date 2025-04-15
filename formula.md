## 公式模板 ##

公式统一使用图片导入，步骤如下：

1. 从PPT编辑公式并导出图片；
2. 放到公式对应文件夹下(LiMapper在根目录下Images/Formula文件夹)；  

### 格式 ###
#### 独立公式 ####
 
高度设置：每行高度30，如下图公式为7行，则总高度为7*30=210。  
左对齐：
  
<div align="left"> 
<img src="../Images/Formula/CameraModel.png" height="210"></img> 
</div>
  
	<div align="left">
	<img src="../Images/Formula/CameraModel.png" height="210"></img>
	</div>
居中：
  
<div align="center"> 
<img src="../Images/Formula/CameraModel.png" height="210"></img> 
</div>
	<div align="center">
	<img src="../Images/Formula/CameraModel.png" height="210"></img>
	</div>
右对齐：

<div align="right">
<img src="../Images/Formula/CameraModel.png" height="210"></img>
</div>

	<div align="right"> 
	<img src="../Images/Formula/CameraModel.png" height="210"></img> 
	</div>

#### 行内公式 ####
 
高度设置：20    
例：式中的<img src="../Images/Formula/CameraModel_1.png" height="20" style="vertical-align:middle"></img>表示

	<img src="../Images/Formula/CameraModel_1.png" height="20" style="vertical-align:middle"></img>  

#### MARKDOWN 原生格式 ####
x =  X ⁄ Z  
y =  Y ⁄ Z  
r = √( x^2+y^2 )  
x' = x(1+K<sub>1</sub>r<sup>2</sup> + K<sub>2</sub>r<sup>4</sup> + K<sub>3</sub> r<sup>6</sup>) + 
   P<sub>1</sub>( r<sup>2</sup> + 2x<sup>2</sup>) + 2P<sub>2</sub>xy   
y' = y(1+K<sub>1</sub>r<sup>2</sup> + K<sub>2</sub> r<sup>4</sup> + K<sub>3</sub>r<sup>6</sup>) + 
   P<sub>2</sub> (r<sup>2</sup> + 2y<sup>2</sup>) + 2P<sub>1</sub>xy  
u = w\*0.5 + c<sub>x</sub> + x'f + x' b<sub>1</sub> + y'b<sub>2</sub>  
v = h\*0.5 + c<sub>x</sub> + y'f

	x =  X ⁄ Z  
	y =  Y ⁄ Z  
	r = √( x^2+y^2 )  
	x' = x(1+K<sub>1</sub>r<sup>2</sup> + K<sub>2</sub>r<sup>4</sup> + K<sub>3</sub> r<sup>6</sup>) + 
	   P<sub>1</sub>( r<sup>2</sup> + 2x<sup>2</sup>) + 2P<sub>2</sub>xy   
	y' = y(1+K<sub>1</sub>r<sup>2</sup> + K<sub>2</sub> r<sup>4</sup> + K<sub>3</sub>r<sup>6</sup>) + 
	   P<sub>2</sub> (r<sup>2</sup> + 2y<sup>2</sup>) + 2P<sub>1</sub>xy  
	u = w\*0.5 + c<sub>x</sub> + x'f + x' b<sub>1</sub> + y'b<sub>2</sub>  
	v = h\*0.5 + c<sub>x</sub> + y'f

## 欢迎继续补充此文档 ##