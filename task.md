# 高级算法最短路径Arboreal-Ants

## 1.总体任务

用C/C++实现simulation的testbed。
对各种图（提供了数据集）进行实验，讨论影响蚁群收敛到最短路径的因素。

影响因子：决策、泄露、流速


### 作业要求：
- 分别实现线性决策下增速与不增速的情况（用表格统计最终收敛到最短路径的实例个数）。
- 对比线性决策下存在泄露与不存在泄露的情况（统计最终收敛到最小泄露路径的实例个数）。
- 至少讨论一种非线性决策下增速和泄露的影响（例如可以给出上一页的实验图）。
- 一组一份实验报告，内容包括源代码描述、实验设置、实验结果、实验结论。

### 数据集
- 包含1000张图。每张图有100个结点，都以邻接矩阵的形式保存在txt文件当中。
- 图的类型包括gnp，gnp_loc，grid三种
- 十种子类型：
gnp_w_loop_w_leakage_0
gnp_w_loop_wo_leakage_0
gnp_wo_loop_w_leakage_0
gnp_wo_loop_wo_leakage_0
gnpLoc_w_loop_w_leakage_0
gnpLoc_w_loop_wo_leakage_0
gnpLoc_wo_loop_w_leakage_0
gnpLoc_wo_loop_wo_leakage_0
grid_wo_loop_w_leakage_0
grid_wo_loop_wo_leakage_0

### 具体
- 根据图是否有环、是否考虑泄露（不考虑泄露表示图中生成了一条唯一的最短路径，这种实例适用于测验蚁群最终能否收敛到最短路径；考虑泄露的实例可能有多条最短路径，适用于测验蚁群最终能否收敛到最小泄露路径），数据集可再细分为10种类别，每种类别有100个实例。（没搞懂这个

- 探究增速影响时，总共使用without leakage的500个实例；探究泄露影响时，总共使用with leakage的500个实例。单次实验跑单个类别的100个实例，在报告中说明这个类别。

- 对于gnp和gnpLoc这两种图，我们按论文种的描述分别把p设置为0.1和0.5（对于前50个实例p设为0.1，后50个则设为0.5）。

- 可选择自己生成更多的图以进行实验，需要注明生成方法以及相关参数。（不做吧

### 评分标准：
算法实现是否合理，运行可执行文件的结果是否与实验报告描述统一。
实验报告总体的呈现效果，包括算法描述、实验结果展示等。

### 加分项：
运行可执行文件整体的效率。
实验丰富程度，更深入的研究与实验（例如信息素初始化，单向流等）。

## 2.分工

### 代码改写
- decision_rules.py 45行
- gen_graph.py 54行
- helper.py 147行
- plot.py 66行
- schema.py 78行
- sim.py 66行
- main.py 265行

可以挑自己熟悉的改，改之前通知一下对方，改好的代码都放ccode文件夹吧

### 实验测试


### 报告部分



## 3.进度
### 预期
- 4.16 讨论代码分工和具体任务
- 4.23 周五前改好C++代码，周末一起调一下跑通
- 4.30 跑各种实验测试效果
- 5.5 写好报告
- 5.7 提交报告

### 实际



## 4.宋


## 5.许