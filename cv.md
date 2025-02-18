# 李建 | 研究助理

📧 lijianonwork@126.com | 💻 [GitHub:lijianfromearth](https://github.com/lijianfromearth/lijianfromearth)  
📍 上海 | 🎓 天津财经大学 计算机科学与技术学士（2020）

---

## 教育背景
**天津财经大学**  
计算机科学与技术 学士 | 2016 - 2020  

---

## 工作经历

### 上海科技大学 MARS 实验室 | 研究助理  
*2024 - 至今 | 导师：Sören Schwertfeger 教授*  

### 中国工商银行软件开发中心（北京） | 应用支持工程师  
*2021 - 2022*  
- 负责维护工行企业网银服务程序和审核版本变动

### 天津华来科技 | Android开发工程师  
*2018*  
- 编写智能摄像头在安卓设备的控制程序  
---

## 论文
**High-Quality, ROS Compatible Video Encoding and Decoding for High-Definition Datasets**  
*Li, Jian | Xu, Bowen | Schwertfeger*  
ROBIO 2024   
- 提出面向ROS系统的视频编解码优化方案  
- 实现55倍压缩比提升，保持SLAM数据集质量  
- 开发自动化处理脚本，提升数据集处理效率

---

## 机器人项目经验

### 基于语义感知的6自由度Affordance抓取姿态生成
*（进行中） 2024.12 - 至今*  
- 项目目标是改进ICRA 2024论文Language-Conditioned Affordance-Pose Detection in 3D Point Clouds  
- 修改原论文Diffusion 架构为DP3架构，并基于此测试diffusion和FlowMatching训练效果。最终选择FM，因其可以更快速的去噪，有利于配合RL微调。  
- 解决条件不显著带来的生成位置错误问题。测试了点云与点云、点云与文本，使用cross attention和拼接特征等不同条件组合，最终选择torch.cat拼接点云与文本特征。  
- 且经实验发现在训练位姿生成时，同时训练Affordance点云区域预测，可增强pointnet++点云特征的表现能力，使得diffusion可以在更多物体上生成正确抓取位姿。  
- 用每次生成50个位姿取代原论文预测单一位姿的方案。经实验发现利用50个位姿的内在约束可以提高模型的收敛速度和生成效果。  
- 目前在小规模的数据集测试中，我们模型的生成效果已超越了原论文需要采样2000次才可筛选出可用位姿的生成效果。相信经过微调我们的模型可以实现**90%**抓取姿态正确率。   
- 开发Fetch Robot控制程序为实机验证做准备。   



### 四足机器人直立抓取系统开发
*（进行中） 2024.02 - 至今*  
- 实现Unitree GO2四足机器人直立平衡控制  
- 设计无指令自主站立算法，优化质心轨迹规划  
- 开发基于强化学习的步态生成系统  



### 基于3D高斯飞溅的灵巧手抓取系统
*2024.08 - 2024.10*  
- 改进RAL 2024论文方法，集成3D高斯预测网络  
- 开发动作镜像系统，实现左右手策略迁移（成功率提升27%）  
- 加速强化学习训练过程（单次迭代时间减少18%）  


### SLAM数据集构建与优化
*2024.04 - 至今*  
- 搭建上海科技大学校园SLAM数据集（包含Faro高精度点云）  
- 开发动态物体标注系统（点云比对法）  
- 设计自动压缩流水线，支持ROS数据集高效存取

---

## 技术栈
**机器人开发**  
ROS/ROS2 | Gazebo | RVIZ | MoveIt  

**机器学习**  
PyTorch | Diffusion Models | RL (PPO, SAC)  

**编程语言**  
Python | C++ | MATLAB  

**工具链**  
Docker | Git | OpenCV | PCL

---

## 荣誉奖励
（建议补充机器人/AI相关竞赛奖项、奖学金等）
