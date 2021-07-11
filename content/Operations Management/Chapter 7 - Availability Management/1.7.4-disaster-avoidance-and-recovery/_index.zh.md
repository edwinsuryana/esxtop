---
title: "4. 灾难避免和恢复"
date: 2021-06-14T14:34:24+10:00
draft: false
weight: 40
---

{{% notice 信息 %}}
本页出租。这意味着我们需要一位贡献作者！
{{% /notice %}}

处理灾难恢复时有 3 个主要用例：

#### 避灾

您可以通过在延伸的 vSphere 集群上执行远程 vMotion 来避免灾难。

- 你有足够的 WAN 带宽吗？
- vMotion 是否在预期时间内完成？ - 如果不是，是什么原因造成的？
- vMotion 期间的性能影响是什么？由于管道是共享的，这也会影响其他虚拟机。

#### DR 测试

您正在按照监管机构或内部业务连续性计划的要求进行测试。您的生产 VM 仍在运行，因此您需要对网络进行冒泡。

- 您在恢复站点上是否有足够的资源？
- 是否在预期时间内完成？如果不是，是什么原因造成的？

#### DR 实际

你正在做实际的恢复。这可以是计划的或计划外的。

- 你有足够的资源吗？
- 对目标集群和数据存储有什么性能影响？

在大型环境中，您可以让多个集群参与主动/主动 DR，相互保护。这会创建复杂的关系，尤其是当您有数百个业务应用程序并且它们跨集群时。