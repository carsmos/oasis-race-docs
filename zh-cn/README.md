
# 1 比赛概览

## 1.1 比赛介绍

<font size=4 color="#cc66ff">2023元遨全球开源自动驾驶算法大赛</font> 基于[元遨开源项目](https://www.carsmos.cn)的自动驾驶仿真平台 [Oasis](https://guardstrike.com/sim.html) 和中间件 [Dora](https://github.com/dora-rs)，在仿真环境下为参赛队伍提供多个预定义的场景，通过不同的场景测试每个参赛队提交的自动驾驶算法在城市区域内各种复杂交通环境下的感知、规划和决策能力。仿真竞赛优胜队伍将被邀请参加**线下车辆挑战赛**。

<!-- 对于每个场景，由参赛选手的算法控制的自动驾驶车辆将在一个起点被初始化，并被指示开往预定义的终点。 场景包含天气、光照条件、交通流（车辆、行人）、红绿灯、交通标志、路障等各种元素。 -->

参赛选手的算法需要合理利用系统提供的各种 [**场景信息**](zh-cn/scenarios.md) 和 [**传感器信息**](zh-cn/start.md#_223-重写-sensors-方法)，使算法控制的主车顺利通过这些预定义场景，并且争取在各个 [**评价指标**](zh-cn/rules.md#_321-评价指标) 上获得更高的得分。

## 1.2 比赛流程

1. [**比赛报名**](https://)

2. [**点击此处下载Oasis竞赛版**](https://carsmos.oss-cn-chengdu.aliyuncs.com/carsmos.tar.gz)，根据 [__安装文档__](zh-cn/install.md)，安装运行 `Oasis` 竞赛版。

3. 基于 [**Oasis**](https://guardstrike.com/sim.html) 和 [**Dora-drives**](https://github.com/dora-rs/dora-drives) 开发和测试自动驾驶算法，参考 [__开发指南__](zh-cn/start.md)。

4. 在 [**算法提交系统**](https://) 中提交算法并等待结果，参考 [**提交镜像**](zh-cn/submit.md)。

## 1.3 比赛帮助和答疑

如果参赛选手对本次开源自动驾驶算法大赛有任何意见或建议，请通过以下渠道与我们联系。

- 邮箱：race@carsmos.ai

<!-- 
如果参赛选手在参赛过程中有任何疑问，欢迎加群讨论

- **钉钉**扫描下方二维码入群：
  
  ![二维码](../images/QRcode.png) -->

## 1.4 文档目录

- [安装部署](zh-cn/install.md)

- [开发指引](zh-cn/start.md)

- [比赛规则](zh-cn/rules.md)

- [提交说明](zh-cn/submit.md)

- [场景说明](zh-cn/scenarios.md)

- [License导入说明](zh-cn/license.md)

<!-- - [报名系统操作说明](zh-cn/signup.md) -->

- [声明条款](zh-cn/clause.md)