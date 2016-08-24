# 历史

![](image/history/history.png)[链接](http://midlab.diag.uniroma1.it/articoli/paper%2066.pdf)


## 第一代
最开始的流处理系统要么是简单的原型、要么是已有数据库引擎的扩展实现（如基于触发器）。通常视为了一些特定的应用场景定制开发，支持的操作非常有限，而
stream processing systems have been built
as stand-alone prototypes or as extensions of existing database engines. They were developed with a specific
use case in mind and are very limited regarding
the supported operator types as well as available functionalities
实现的逻辑一般是简单地基于静态规则（Rule）的触发，包括：
条件（Condition）
时间（Timer）
事件（Event）

配置状态无关
简单粗暴的实现却是经济有效的办法。

<u>**简单事件处理（SEP，Simple Event Processing）**</u>
## 第二代

随着场景的复杂，处理逻辑对于上下文状态有依赖，因此要求
1. 能保留流处理的状态
2. 处理系统有较高的容错能力（fault tolerance），能在故障后恢复状态
3. 静态配置编排变成语言编译，

<u>**复杂事件处理（CEP，Complex Event Processing）**</u>


事件、事务

更加丰富的语义
systems extended the ideas of data
stream processing with advanced features such as fault
tolerance [1], adaptive query processing [34], as well
as an enhanced operator expressiveness [7]. Important
examples of this class are Borealis [1], CEDR [7], System
S [22] and CAPE [34].


## 第三代
第三代的流处理系统是随着云计算以及大数据的兴起而诞生的，其设计要求引擎有非常好的可扩展能力和更加鲁棒的容错能力。
system design is strongly driven by the
trend towards cloud computing, which requires the
data stream processing engines to be highly scalable
and robust towards faults. Well-known systems of
this generation include Apache S4 [30], D-Streams [42],
Storm [27] and StreamCloud [18].

日志处理（大数据）

## 流处理系统与复杂事件处理系统的对比

| 0:0 | 1:0 | 2:0 |
| -- | -- | -- |
| 0:2 | 1:2 | 2:2 |
| 0:3 | 1:3 | 2:3 |
| 0:4 | 1:4 | 2:4 |
| 0:5 | 1:5 | 2:5 |
| 0:6 | 1:6 | 2:6 |
| 0:7 | 1:7 | 2:7 |
| 0:8 | 1:8 | 2:8 |
| 0:9 | 1:9 | 2:9 |
| 0:10 | 1:10 | 2:10 |

## 参考资料

1. [Tutorial: Cloud-based Data Stream Processing](http://midlabTutorial: Cloud-based Data Stream Processing.diag.uniroma1.it/articoli/paper 66.pdf)
