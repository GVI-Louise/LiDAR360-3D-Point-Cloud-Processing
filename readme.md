# LiDAR360 手册写作说明

## 模板 ##

- 功能介绍参照[功能介绍模板](功能介绍模板.md)
- 流程操作参照[流程操作模板](流程操作模板.md)
- 文档结构参照[SUMMARY](SUMMARY.md)

## 句中插图规则 ##

- **种子点文件**：点击<img src="./ScreenShot/universe/ALSForest/ImportData.png" height="20" style="vertical-align:middle"></img>，选择点云数据对应的种子点文件。

## 关于截图 ##

- 上传截图时，如果截图在中英文情况下表现不同，则要同时上传中英文两个版本的，分别放入Images/Screenshot/zh和Images/Screenshot/en文件夹中，名称保持一致。
- 上传截图时，如果截图在中英文情况下表现相同，则放入Images/Screenshot/universe文件夹中。
- 推荐使用Windows 7进行截图。
- 注意图片文件夹及图片名字不要使用中文。
- 需要缩放图片时可采用如下语句（通过raw file查看）

		<div align=center>
		<img src="Icon/LiDAR360-Startup.png" alt="LiDAR360 Startup" width="480"/>
		</div>
<div align=center>
<img src="Icon/LiDAR360-Startup.png" alt="LiDAR360 Startup" width="480"'/>
</div>
- 插入图片会导致有序列表重新排序，需将图片区域缩进。  
### 缩进前： ###
1. 步骤1
<div align="center">
<img src="Icon/LiDAR360-Startup.png" alt="LiDAR360 Startup" width="100"/>
</div>
2. 步骤2
	<br>  
### 缩进后：
1. 步骤1
	<div align="center">
	<img src="Icon/LiDAR360-Startup.png" alt="LiDAR360 Startup" width="100"/>
	</div>
2. 步骤2

## 关于文件链接路径 ##

### 书写格式###
  
- 同一级或下一级目录下文件链接，采用“./xx.md”、“./xx/xx.md”方式。
- 上一级目录文件链接，采用“../xx.md”、“../xx/xx.md”等。  
示例： 

		[Index](./Index.md) [日志面板](./Modules/ConsoleWindow.md)  
[Index](./Index.md) [日志面板](./Modules/ConsoleWindow.md)  		
- 跳转指定章节的某个标题（跳转功能仅在html和pdf格式可见）  
示例：跳转到/Modules/AlignPhotosSettings.md文件中的"平差"标题  
1.在需跳转位置添加语句：

	[影像对齐](./Modules/AlignPhotosSettings.md#6) [影像对齐](./Modules/AlignPhotosSettings.md#6)  
[影像对齐](./Modules/AlignPhotosSettings.md#6) [影像对齐](./Modules/AlignPhotosSettings.md#6)  
2.在标题位置添加语句

	<div id="6"></div>
语句中的id编号6可自行修改，根据标题位置从上到下对其编号，具体可参考“/Modules/AlignPhotosSettings.md”中编号方式。

## 关于LiDAR360与LiMapper模板统一的问题 ##

根据长期计划，LiDAR360与LiMapper将逐步融合，文档也需风格统一。LiDAR360目前模板请参考[功能介绍模板](./Template/LiDAR360/ModuleTemplate.md)、[流程操作模板](./Template/LiDAR360/WorkflowTemplate.md)。

基本框架与LiMapper现行模板类似，但LiDAR360功能更加复杂。LiMapper的流程化处理较为简单，在360模板框架下，可根据实际流程进行删减。比如LiMapper的小功能并没有那么复杂的**原理描述**。

需要注意细节目前有

- 引用大图居中
- 点击菜单栏用到*斜体*，如点击*文件->新建文件*

## 关于引用文献

**引用文献及跳转如下所示**

CHM分割使用分水岭分割算法<a href="#1">(Lee et al., 2010)</a>识别和分割单棵树，获取单木位置、树高、冠幅直径、冠幅面积和树木边界。

**文献标识、作者、名称、期刊、年份写在文档最后，如下所示：**

<div id="2"></div>
		@inproceedings{schoenberger2016sfm,
		    author={Sch\"{o}nberger, Johannes Lutz and Frahm, Jan-Michael},
		    title={Structure-from-Motion Revisited},
		    booktitle={Conference on Computer Vision and Pattern Recognition (CVPR)},
		    year={2016},
		}

## 欢迎继续补充此文档 ##

