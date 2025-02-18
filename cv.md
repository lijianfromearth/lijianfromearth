# 李健 | 科研助理

📧 lijianonwork@126.com | 💻 [GitHub:lijianfromearth](https://github.com/lijianfromearth/lijianfromearth)  
📍 上海 | 🎓 天津财经大学 计算机科学与技术学士（2020）

---

### 教育背景
**天津财经大学**  
计算机科学与技术 学士  Cet6 | 2016 - 2020  

---

## 工作经历

**上海科技大学 MARS 实验室 | 科研助理**  
*2024 - 至今 | 导师：Sören Schwertfeger 教授*  

**中国工商银行软件开发中心（北京） | 应用支持工程师**  
*2021 - 2022*  
- 负责维护工行企业网银服务程序和审核版本变动

**天津华来科技 | Android开发工程师**  
*2018*  
- 编写智能摄像头在安卓设备的控制程序  
---

### 论文
**High-Quality, ROS Compatible Video Encoding and Decoding for High-Definition Datasets**  
*Li, Jian | Xu, Bowen | Schwertfeger*  
ROBIO 2024   

---

### 机器人项目经验

### 基于语义感知的6自由度Affordance抓取姿态生成
*（进行中） 2024.12 - 至今*  
- 项目目标是改进ICRA 2024论文Language-Conditioned Affordance-Pose Detection in 3D Point Clouds  
- 修改原论文Diffusion架构为DP3架构，并基于此测试diffusion和FlowMatching训练效果。最终选择FM，因其可以更快速的去噪，有利于配合RL微调。测试发现FM仅3步预测即可达到Diffusion的去噪效果。    
- 解决条件不显著带来的生成位置错误问题。测试了点云与点云、点云与文本，使用cross attention和拼接特征等不同条件组合，最终选择torch.cat拼接点云与文本特征。  
- 且经实验发现在训练位姿生成时，同时训练Affordance点云区域预测，可增强pointnet++点云特征的表现能力，使得diffusion可以在更多物体上生成正确抓取位姿。  
- 用每次生成50个位姿取代原论文预测单一位姿的方案。经实验发现利用50个位姿的内在约束可以提高模型的收敛速度和生成效果。  
- 目前在小规模的数据集测试中，我们模型的生成效果已超越了原论文需要采样2000次才可筛选出可用位姿的生成效果。相信经过微调我们的模型可以实现**90%**抓取姿态正确率。   
- 开发Fetch Robot控制程序为实机验证做准备。   



### 四足机器人直立抓取
*（进行中） 2025.02 - 至今*  
- 负责实现Unitree GO2四足机器人直立平衡和行走步态   
- 使用控制指令混合训练的策略在无指令时无法稳定直立，目前负责在此预训练基础上做微调以实现行走和无指令时的稳定站立。    



### 基于3D高斯的灵巧手抓取
*2024.08 - 2024.10*  
- 基于论文“RESPRECT:Speeding-up Multi-fingered Grasping with Residual Reinforcement Learning“，负责引入高斯基元作为视觉特征。
- 负责训练高斯预测网络，以加速RL训练时的高斯推理。  
- 开发镜像程序，实现将右手抓取策略部署到左手执行。  
- 编写程序使用Pyk4A 读取远程kinect深度图数据，使用FoundationPose实现目标姿态跟踪。  
- 测试发现直接从零开始训练抓取成功率很难上升，使用预设的抓取动作从演示中学习可加速RL训练。（不幸该项目夭折，未完成训练）



### ShanghaiTech Mapping Robot 数据集
*2024.04 - 至今*  
- 使用ShanghaiTech Mapping Robot收集校园SLAM数据集和Faro高精度点云数据集。  
- 测试在保持SLAM数据集视觉感知质量情况下的最优参数，实现55倍压缩，产出一篇ROBIO论文。    
- 编写数据集压缩程序，将Rosbag数据转化为mp4视频和保存必要参数的yaml文件。编写压缩数据集播放脚本，支持常规Rosbag播放命令。
- 将Faro点云作为真值，编写程序对比Mapping Robot数据集标注动态物体。（目前的工作）  

---

### 技术栈
RL | diffusion | Ros | OrbSlam2 | Android | Web | Java/C++/Python

