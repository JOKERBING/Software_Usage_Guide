# Altium Designer 24 PCB 走线倒圆弧方法

在 PCB 设计中，走线转角过于尖锐不仅影响美观，还可能引起信号完整性问题。本文介绍如何在 Altium Designer 24 中通过倒圆弧优化走线，使设计更趋完美。

## 问题描述

在设计过程中，我们常会遇到走线转角过于锐利的问题，这可能会引发制造难度和电气性能方面的隐患。如何快速、精准地对现有 PCB 走线进行倒圆弧处理，从而提升整体设计质量，是本文要解决的关键问题。

## 解决方法

### 设置倒圆弧参数

首先，在【设置】栏中找到【PCB Editor】下的【Gloss and Retrace】选项，并进行如下设置：

【环抱风格】设置为【Rounded】，【Effort】设置为【Weak】。

<div align=center><img src="Altium Designer 24 PCB 走线倒圆弧方法/微信截图_20250331170618.png" width="800"></div>

### 选择需要优化的走线

打开 PCB 编辑器右侧的【Properties】栏，在过滤器【Selection Filter】中只选择【Tracks】。

按住 SHIFT 键，同时框选所有需要倒圆弧处理的走线，以便将这些对象批量选中。

<div align=center><img src="Altium Designer 24 PCB 走线倒圆弧方法/微信截图_20250331170835.png" width="600"></div>

### 进行走线优化

在【布线】栏中选择【优化选中走线】。系统会自动对选中的走线进行倒圆弧处理，从而改善走线转角。

<div align=center><img src="Altium Designer 24 PCB 走线倒圆弧方法/屏幕截图1.png" width="800"></div>

## 优化效果展示

优化前：

<div align=center><img src="Altium Designer 24 PCB 走线倒圆弧方法/微信截图_20250331172059.png" width="800"></div>

优化后：

<div align=center><img src="Altium Designer 24 PCB 走线倒圆弧方法/微信截图_20250331172042.png" width="800"></div>
