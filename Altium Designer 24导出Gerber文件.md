# Altium Designer 24导出Gerber文件

Gerber（光绘）文件是一种符合EIA标准、用于驱动光绘机的文件。通过该文件，可以将PCB中的布线数据转换为光绘机用于生产1:1高度胶片的光绘数据。当使用Altium Designer 24绘制好PCB电路图文件之后，需要打样制作，但又不想提供给厂家工程文件，那么就可以直接生成Gerber文件，然后将其提供给PCB生产厂家，就可以打样制作PCB板。

输出Gerber文件时，建议在工作区打开扩展名为`.PrjPcb`的工程文件，生成的相关文件会自动输出到`Project Outputs for ***`文件夹中。

其主要操作有如下四步：

## 1、输出Gerber文件

在PCB界面中，执行菜单栏中的【文件】→【制造输出】→【Gerber Files】命令。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104151039.png" width="1000"></div>

在弹出的【Gerber Setup】对话框中，【Units】选择【Inches】,【Outputs:FileName.Extension】选择【*.gbr】。

切换到【Layers to plot】选项卡，在【Plot Layers】上拉列表中选择【Select Used】选项，然后检查需要输出的层。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104151206.png" width="800"></div>

切换到【Advanced】选项卡，勾选【Generate DRC Rules export file(.RUL)】复选框，之后单击【Apply】按钮。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104151326.png" width="800"></div>

得到输出预览后直接关闭预览即可。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104151409.png" width="1000"></div>

无需保存，单击【Don't Save】按钮。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104165955.png" width="400"></div>

## 2、输出NC Drill Files钻孔文件

切换回PCB编辑界面，执行菜单栏中的【文件】→【制造输出】→【NC Drill Files】命令，进行过孔和安装孔的输出设置。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170042.png" width="1000"></div>

在弹出的【NC Drill设置】对话框中，【单位】选择【英寸】,【格式】选择【2:4】，勾选【摒弃前导零】复选框，勾选【生成EIA二进制钻孔文件(.DRL)】复选框，单击【确定】按钮。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170112.png" width="800"></div>

弹出多个【导入钻孔数据】对话框，直接单击【确定】按钮即可。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170155.png" width="400"></div>

得到输出预览后直接关闭预览即可。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170219.png" width="1000"></div>

无需保存，单击【Don't Save】按钮。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170222.png" width="400"></div>

## 3、输出Test Point Report IPC网表文件

切换回PCB编辑界面，执行菜单栏中的【文件】→【制造输出】→【Test Point Report】命令，进行IPC网表文件输出。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170249.png" width="1000"></div>

在弹出的【Fabrication Testpoint Setup】对话框中，勾选【IPC-D-365A】复选框，单击【确定】按钮。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170327.png" width="600"></div>

弹出多个【导入钻孔数据】对话框，直接单击【确定】按钮即可。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170328.png" width="400"></div>

得到输出预览后直接关闭预览即可。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170330.png" width="1000"></div>

无需保存，单击【Don't Save】按钮。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170331.png" width="400"></div>

## 4、输出Generates pick and place files坐标文件

切换回PCB编辑界面，执行菜单栏中的【文件】→【装配输出】→【Generates pick and place files】命令，进行坐标文件输出。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170600.png" width="800"></div>

在弹出的对话框中进行相应设置，【单位】勾选【英制】复选框，【格式】勾选【CSV】复选框，单击【确定】按钮即可输出坐标文件。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104170810.png" width="800"></div>

至此，Gerber文件输出完成。输出过程中产生3个`.cam`文件可直接关闭，不用保存.

## 输出内容Project Outputs for *** 文件夹

在工程目录下的Project Outputs for ***文件夹中的文件即为Gerber文件。将其重命名，打包成压缩包发给PCB生产厂商制作即可。

<div align=center><img src="Altium Designer 24导出Gerber文件/20240104184429.png" width="1000"></div>