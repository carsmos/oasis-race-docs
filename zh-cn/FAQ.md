# 10 常见问题
## 10.1 关于比赛

- 本次比赛比的是感知还是决策？

    本次比赛的内容是全闭环测试，而您可以自由选择进行感知优化或决策优化。系统中会搭载整套基本的感知决策算法，您可以选择擅长的部分进行优化和替换。

## 10.2 报名参赛
- 谁可以报名？

    只要您有一定的编程基础，对自动驾驶技术感兴趣，就欢迎报名。

- 队伍成员数量有没有限制？

    当前一个队伍的成员数量是没有被限制的，您可以按照自己的想法添加队员。

- 报名成功后在哪里可以看到队伍信息？

    在这里可以看到您的队伍及成员信息：[算法提交平台](https://race.carsmos.cn/)

- 报名成功后还能添加新的队员吗？

    目前没有支持这个功能。如果有您的朋友希望参与比赛，可以另外报名构建一个新的队伍。

## 10.3 安装与运行 Oasis
- 怎么申请 License ？

    双击桌面图标进入 Oasis 系统后，点击 “申请 License” 按钮并输入相关信息，License 文件会被自动发送至您填写的邮箱。从邮箱下载 License 文件并导入 Oasis 即可。

- 进入 Oasis 后提示“网络连接失败”怎么办？

    这是由于 Oasis 需要的一些端口被其他程序占用了，在安装之前，需要检查端口是否被占用，参考：[**安装步骤**](zh-cn/install.md#_22-安装步骤)。

    网络问题解决后，可以使用 Ctrl+Shift+R 刷新页面。

- 任务为什么会一直显示“排队中”？

    1. 安装不成功（正常情况下有11个运行正常的容器），请关注安装情况，同时 docker ps -a 查看各个容器是否运行状态正常
    2. 检查输出日志，看是否有错误
        ```
        docker logs -f oasis-task-manager
        ```
    3. 安装机器有没有安装nvidia驱动，可以通过 nvidia-smi来查看是否安装驱动

- 任务为什么会运行“异常”
    
    1. 可能由于代码错误。您可以检查代码是否有语法错误
    2. 可能由于任务超时（超时时间为8分钟），即在规定的时间内主车没有到达终点。
    3. 可能由于carla未正常启动。检查carla是否正常启动（检查nvidia驱动是否安转正常`nvidia-smi`）：
        ```
        docker logs -f oasis_carla_0.9.13-0407
        ```
    4. 通过 
        ```
        docker ps -a
        ```
        检查任务运行过程中 carla 是否有过重启（检查 STATUS 状态）