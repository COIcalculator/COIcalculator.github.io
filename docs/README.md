# daxfb-calculator
工厂管理游戏的计算器/工厂规划工具。

[此页面的链接](https://doubleaxe.github.io/daxfb-calculator/docs/).

[编辑此页面](https://github.com/doubleaxe/daxfb-calculator/edit/main/docs/README.md).

# 通用用法

计算器可以在两种模式下工作：`拖放模式` 和 `点击模式`。
第一种针对 PC 使用进行了优化，默认在 PC 上打开。
第二种针对移动设备进行了优化（和默认使用），但也可在 PC 上使用。
模式可通过`选项`对话框切换打开和关闭。

## 拖放模式

在此模式下，一切都通过鼠标主键拖动。
注意：如果同时启用 `拖放` 和 `点击` 模式,
鼠标按钮在项目上按下和拖动实际开始之间会有延迟（300 毫秒）。
这样做是为了区分 `点击` 和 `拖动` 事件。

<details><summary>拖动工厂并放在蓝图上</summary>

![drag-n-drop-1](./assets/drag-n-drop-1.gif)
</details>

<details><summary>在工厂之间拖动链接</summary>

![drag-n-drop-2](./assets/drag-n-drop-2.gif)
</details>

<details><summary>拖动链接以更改端口排序</summary>

![drag-n-drop-6](./assets/drag-n-drop-6.gif)
</details>

<details><summary>拖动以移动工厂</summary>

![drag-n-drop-3](./assets/drag-n-drop-3.gif)
</details>

<details><summary>在空闲空间上拖动以滚动窗口</summary>

![drag-n-drop-4](./assets/drag-n-drop-4.gif)
</details>

<details><summary>拖动东西超出窗口以自动滚动</summary>

![drag-n-drop-5](./assets/drag-n-drop-5.gif)
</details>

## 点击模式

在此模式下，可以通过点击选择项目，然后通过另一次点击目标元素来粘贴/移动。

<details><summary>在蓝图上粘贴工厂</summary>

![point-n-click1](./assets/point-n-click1.gif)
</details>

<details><summary>在工厂之间粘贴链接</summary>

![point-n-click2](./assets/point-n-click2.gif)
</details>

<details><summary>更改端口排序（应小心点击端口之间的空闲空间）</summary>

![point-n-click4](./assets/point-n-click4.gif)
</details>

<details><summary>移动工厂</summary>

![point-n-click3](./assets/point-n-click3.gif)
</details>

# 选择配方

只需点击中心工厂图标选择配方。筛选器也在这里工作。
如果工厂只有一个配方-不会显示配方菜单。

<details><summary>详情</summary>

![recipe-selection](./assets/recipe-selection.png)
</details>

# 工厂旋转

可以旋转工厂以创建更漂亮的链接。

<details><summary>实际操作</summary>

![rotation](./assets/rotation.gif)
</details>

# 工厂计数调整

工厂计数可以使用汉堡菜单设置。可选择在设置中打开工厂卡片上的加号和减号按钮。加号和减号调整计数，而菜单上的文本框可用于设置分数计数。还有工具栏上的批量更新计数按钮，可用于应用自动计算的计数。

<details><summary>实际操作</summary>

![count-adjustment](./assets/count-adjustment.gif)
</details>

# 工厂升级/降级

如果工厂有下一个或上一个等级版本，升级选项在汉堡菜单内可用。打开升级模式可影响所有工厂。

<details><summary>实际操作</summary>

![upgrade-mode](./assets/upgrade-mode.gif)
</details>

# 物流运输检查

物流运输可以检查链接，这些链接与已知运输（输送机、管道、操纵器、机械臂）连接项目。单击链接菜单时，物流信息将自动显示。特定运输可以被锁定，在这种情况下，整个蓝图将更喜欢锁定的运输。

<details><summary>实际操作</summary>

![logistic](./assets/logistic.gif)
</details>

# 摘要窗口

摘要窗口将显示蓝图的总体消耗/生产/建筑成本。由于在更新蓝图时进行计算-对于非常大的蓝图，建议将其关闭。摘要窗口可以以两种模式工作-简单和扩展。模式通过相应的按钮依次切换。如果蓝图为空或未计算，摘要窗口将为空。摘要窗口仅显示打开端点的生产/消耗（未连接到任何东西）。


<details><summary>实际操作</summary>

![summary](./assets/summary.gif)
</details>

# 筛选

文本过滤器接受多个单词，这些单词通过空格分开，然后一起应用过滤。
例如搜索文本 `it a` 可用于搜索 `Item A`, 或 `co fu` 可用于搜索 `Copper Blast Furnace`。

## 在左面板上筛选

左面板工厂可以通过输入/输出项目进行筛选。
如果应用过滤-从左面板添加新工厂到蓝图后，将自动选择相应的配方。

## 按蓝图上工厂的输入/输出筛选

显示吞吐量的输入/输出相邻方块可以点击以快速筛选左面板匹配项目。
由于筛选的配方会自动选择，这样长生产线可能更轻松和更快速地建导。

<details><summary>实际操作</summary>

![factory-filtering](./assets/factory-filtering.gif)
</details>

## 在摘要窗口上筛选

也可以通过单击摘要窗口上的图标来应用过滤。

# 求解图

通过单击工具栏按钮 ![solve](./assets/solve.png) 来求解图。
在自动模式下，图会在每次更改时自动求解。
由于对更大的工厂计数求解较慢-对于非常大的蓝图，首选手动模式。

求解使用固定精度进行，可在`设置`中更改。
数字越低，意味着精度越高，准确性越好。
正因为如此，如果连接的工厂吞吐量差异很大或精度太低，将会出现计算错误。

## 自动图形错误检测

当工厂输出两种项目类型，并且这些项目直接或通过生产链会以不同比率馈送到另一工厂时，工厂链可能会不平衡。生产周期也可能不平衡。在这种情况下，图形求解器无法求解工厂io，因此整个流量将为 0。这是预期的，因为这种类型的真实生产链在一段时间后也会以零速率生产，因为一个输出将被堵塞或输入将被挨饿。

图形求解器具有自动错误检测，并将尝试找到导致错误的端口。这通过向每个工厂输出添加具有最低优先级的虚拟接收器来实现。如果此虚拟接收器流量不为零，这意味着连接的工厂输出不平衡，这样的输出将以红色突出显示。要解决此错误，应添加一些建筑而不是此虚拟接收器，这将消耗溢出的项目。

仅自动检测不平衡的输出，因为这是最常见的情况。

<details><summary>示例</summary>

![unbalanced-graph](./assets/unbalanced-graph.gif)
</details>

## 特殊建筑

几乎每个游戏实现都有一套特殊建筑。这些建筑通常表示为容器（可能在真实游戏中不存在），它接受某种项目（流体、固体等）。这些建筑有 3 个配方，输入、输出和输入+输出。它们可以用作实用建筑来调整生产流或具有更好的图形布局。

# 微调图形求解过程

## 锁定工厂

最初，如果给定行中的工厂都没有被锁定，没有输入/输出可以超过最大值。
在此模式中，计算器将回答以下问题：瓶颈在哪里，这条线将生产多少种品。

当一个或多个工厂被锁定时，此行中的其他工厂可以超过其最大计数。
在此模式中，计算器将回答以下问题：此速率下需要多少工厂来生产物品。

<details><summary>实际操作</summary>

![locking](./assets/locking.gif)
</details>

## 设置目标

最初使用简单模式计算图形。在这种模式下，图形求解器尝试最大化整体io流。这对于简单的生产链是可以接受的，但对于具有多个相关输出的复杂链可能会调整，其中最大化一个输出将最小化其他。建议仅以一个最终产品作为主要目标。图形求解器将首先最大化主要目标，然后将尝试最大化次要目标而不损害主要目标。如果将任何工厂设置为目标-所有其他工厂都从最大化过程中排除。

<details><summary>实际操作</summary>

![locking](./assets/objective.gif)
</details>

# 已知问题和限制

## 连接工厂之间流量差异过大

当一个工厂生产/消耗比例远高于另一个连接工厂（1000 倍或更多），并且其数字不是整数时，由于精度不足，计算器无法确定正确的计数。为了解决此问题，应将精度设置为其他（更低）值，尽管对于某些情况可能不够。
