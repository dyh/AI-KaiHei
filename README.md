# AI-KaiHei
和AI队友开黑，打游戏！

## 简介

项目中文名称：AI开黑

项目英文名称：AI Kai Hei

项目方向：人工智能 开黑 游戏队友

短期目标：用 人工智能 玩荒野乱斗游戏 和 自己开黑

运行环境：项目运行在windows10上，android模拟器 + windows 10


## todo list

#### 一、开发环境配置 部分

1、开发环境：cuda、opencv、pycharm、pytorch、labelImg。

2、运行环境：android模拟器、虚拟摇杆配置、荒野乱斗游戏。

#### 二、游戏主程 部分

1、python 控制 荒野乱斗游戏 人物 按照设定的方向移动。

2、python 控制 荒野乱斗游戏 人物 按照设定的方向射击。

3、设定 游戏各个阶段 的 开始信号 和 结束信号。

4、根据 游戏流程，python控制 自动点击 相应的按钮，自动化执行所有 开始、继续、退出 等 非战斗操作。

5、控制 何时激活 卷积神经网络 进行目标检测。

6、根据 通过卷积神经网络 识别到的物体信息，进行相关的业务逻辑操作。

例如 

（1）控制 荒野乱斗游戏 人物 跟随队友、与队友保持距离、寻路，自动绕过墙壁、栅栏、墓碑 等。

（2）控制 荒野乱斗游戏 人物 与敌方保持距离。自动绕过墙壁、栅栏、墓碑 等。

（3）控制 荒野乱斗游戏 人物 按照一定角度攻击 敌方 或 箱子 等。

#### 三、战斗中 实时目标检测 数据集采集和样本标注 部分

1、荒野乱斗游戏 确定有哪些检测的物体类别。例如 对手、队友、自己、墙壁、草地、栅栏、墓碑、箱子 等

2、荒野乱斗游戏 定义有效样本。例如 如何让 卷机神经网络 采集到 对手的某个特征，标注的时候应该标注哪些区域，不应标注哪些区域

3、荒野乱斗游戏 样本采集。例如 玩游戏，录视频，转图片，挑取包含有效样本的图片，待用。

4、荒野乱斗游戏 样本标注，形成训练数据集。

例如

（1）用 labelImg 手工标注图片。

（2）上传至 roboflow.ai导出yolo v5的数据集。

（3）配合 训练卷积神经网络 对 样本标注 进行返工，手工标注图片。

（4）日后，如果训练成功，用 卷积神经网络 识别出的图片，再生成更多的数据集。

#### 四、战斗中 实时目标检测 训练卷积神经网络 部分

1、选择 一种或多种 适合的 卷积神经网络。例如 yolo v5，试验yolo v5自带各种网络的差异性。

2、使用 google colab 对标注完的样本 进行训练。试验 定义的样本是否有效（能否检测得到）

3、如果 训练失败，找出原因，配合 数据集采集和样本标注 对 样本标注 进行返工。

4、如果 训练成功，继续训练下一个目标检测。

#### 五、未来

2个AI队友开黑，共享视野，玩荒野乱斗游戏。


