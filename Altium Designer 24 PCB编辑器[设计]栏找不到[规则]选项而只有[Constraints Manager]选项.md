# Altium Designer 24 PCB编辑器[设计]栏找不到[规则]选项而只有[Constraints Manager]选项

## 问题描述

在使用 Altium Designer 24 的PCB编辑器时，发现有的PCB文件的【设计】栏下有【规则】这个选项，有的PCB文件的【设计】栏下没有【规则】这个选项，取而代之的是【Constraint Management】选项。

下图是带有【规则】选项的PCB文件截图，可以看到在【设计】栏下有【规则】这个选项。

<div align=center><img src="Altium Designer 24 PCB编辑器[设计]栏找不到[规则]选项而只有[Constraints Manager]选项/屏幕截图1.png" width="600"></div>

下图是不带【规则】选项的PCB文件截图，可以看到在【设计】栏下只有【Constraint Management】这个选项。

<div align=center><img src="Altium Designer 24 PCB编辑器[设计]栏找不到[规则]选项而只有[Constraints Manager]选项/屏幕截图2.png" width="600"></div>

## 问题原因

原因是新版的 Altium Designer 中，新增加了采用“Constraints Management”（约束管理）方式管理设计要求，提供更直观和灵活的设置界面。

PCB编辑器【设计】栏找不到【规则】选项的原因是在创建项目时勾选了【Constraint Management】选项。

<div align=center><img src="Altium Designer 24 PCB编辑器[设计]栏找不到[规则]选项而只有[Constraints Manager]选项/微信截图_20250330220016.png" width="800"></div>

## 解决方法

新建一个项目，在创建项目时不要勾选【Constraint Management】选项。

把之前项目中的原理图文件、PCB文件等通过【添加已有的到项目】选项加入到这个新项目中，之后再次打开PCB编辑器，就会发现【设计】栏下出现了【规则】这个选项。

<div align=center><img src="Altium Designer 24 PCB编辑器[设计]栏找不到[规则]选项而只有[Constraints Manager]选项/屏幕截图3.png" width="600"></div>

****

参考资料：

[AD24 找不到“规则”选项](https://blog.csdn.net/Outer_s/article/details/136962977)