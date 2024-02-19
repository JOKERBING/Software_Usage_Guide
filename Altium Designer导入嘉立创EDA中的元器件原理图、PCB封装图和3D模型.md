# Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法

在立创商城找到需要使用的元器件，单击进入详情页。

[立创商城_一站式电子元器件采购自营商城-嘉立创电子商城](https://www.szlcsc.com/)

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130220536.png" width="800"></div>

进入详情页点击右侧【下载文件】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130220748.png" width="800"></div>

点击【立即打开】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130220810.png" width="800"></div>

在打开的立创EDA网页版中分别下载原理图文件（`.schdoc`）和封装图文件（`.pcbdoc`）。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130220924.png" width="800"></div>


<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130220946.png" width="800"></div>

输出文件时单击【导出Altium Designer】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130221035.png" width="600"></div>

之后在立创EDA网页版中新建一个工程，选择【文件】-【新建】-【工程】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130221143.png" width="800"></div>

任意取一个名字或使用默认命名，单击【保存】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130221336.png" width="800"></div>

在该工程下的PCB图中插入需要使用的元器件。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130221454.png" width="800"></div>

选择【文件】-【导出】-【3D文件】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130221524.png" width="800"></div>

勾选【STEP】和【PCB+元件模型】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130221545.png" width="600"></div>

这时导出的3D模型是板子和元器件模型一起的，需要3D建模软件进行一下处理，这里选择使用Fusion 360进行处理，用该软件打开模型。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130222318.png" width="800"></div>

删除板子的模型，只保留元器件的模型，导出为STEP格式文件。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130222728.png" width="800"></div>

使用Altium Designer打开原理图文件（`.schdoc`），选择【设计】-【生成原理图库】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130223511.png" width="800"></div>

在生成的原理图库文件（`.SCHLIB`）中就是该元器件的原理图，复制到自己的库中即可。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130223512.png" width="800"></div>

使用Altium Designer打开封装图文件（`.pcbdoc`），选择【设计】-【生成PCB库】。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130223814.png" width="800"></div>

在生成的封装图库文件（`.Pcblib`）中就是该元器件的封装图，复制到自己的库中即可。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130223815.png" width="800"></div>

在封装页面中点击插入模型图标，选择刚刚用3D建模软件处理过的元器件3D模型。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130224053.png" width="800"></div>

拖动模型并放置在与封装重合的位置上。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130224121.png" width="800"></div>

之后进入3D视图，发现模型悬浮在空中。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130224259.png" width="800"></div>

可以先单击选中模型，通过右侧的【3D Model Type】对三轴角度和元器件高度进行调节。

<div align=center><img src="Altium Designer导入嘉立创EDA中的元器件原理图、PCB封装图和3D模型的操作方法/QQ截图20240130224507.png" width="800"></div>

这样一个元器件的原理图、封装图和3D模型就导入完成了。