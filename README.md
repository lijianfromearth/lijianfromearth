


Hi there 👋  
I am Lijian, a Research Assistant at the shanghaitech MARS Lab, working with Prof. Sören Schwertfeger.  
Currently, my work is focused on **Dexterous Hand Manipulation**, **Diffusion Models**, and **Quadruped Control**.  

Before joining ShanghaiTech, I worked at the Industrial and Commercial Bank of China Software Development Center (Beijing). I obtained my Bachelor Degree in Computer Science and Technology from Tianjin University of Finance and Economics in 2020.  



## Papers  
**High-Quality, ROS Compatible Video Encoding and Decoding for High-Definition Datasets**  
*Li, Jian | Xu, Bowen | Schwertfeger*  
ROBIO 2024  



## Project Experience  

### Generation of 6DOF Grasp Poses using Internal Constraints and Open Semantic Affordance  
*Utilizing Flowmatching and RL (Work in Progress)*  
- Our work aims to improve the generation effect of the 2024 ICRA article *Language-Conditioned Affordance-Pose Detection in 3D Point Clouds*.  
- So far, our pose generation effect has far exceeded that of the article, with **90%** of the generated poses being correct.  
<table>
    <tr>
        <td><img src="./img/LCAP_res.jpeg" alt="LCAP Generation Effect" width="200" height="150"></td>
        <td><img src="./img/our_res.jpeg" alt="Our Model's Effect" width="200" height="150"></td>
    </tr>
</table>
- Left LCAP Generation Effect
- right Our Model's Effect   
- 后续我们将用Fetch Robot 进行实机测试  

### Quadruped Robot Upright Grasping Project  
*(Work in Progress)*  
- Responsible for the training of upright balance and walking gaits for the UNITree GO2.
- 目前专注解决直立步态和无指令时的平衡.
- 
    <tr>
        <td><img src="./img/go2stand1.gif" alt="go2stand1" width="200" height="150"></td>
        <td><img src="./img/go2stand2.gif" alt="go2stand2" width="200" height="150"></td>
    </tr>

### 使用3D高斯的灵巧手抓取  
- 项目基于2024 RAL 论文 RESPRECT: Speeding-up Multi-fingered Grasping with Residual Reinforcement Learning
- 整合高斯泼溅代码到论文代码中，训练高斯集元预测网络加速RL训练过程中的高斯推理
- 编写action和OBS的镜像代码，将右手抓取策略部署到了左手
- 
    <tr>
        <td><img src="./img/lefthandgrasp_gaus.jpeg" alt="go2stand1" width="200" height="150"></td>
        <td><img src="./img/lefthandgrasp_v.gif" alt="go2stand2" width="200" height="150"></td>
    </tr> 

### ShanghaiTech Mapping Robot SLAM 数据集  
- 使用 Mapping Robot 和 Faro 采集校园数据集
- 测试不同的编码器及其设置，以找到压缩视觉SLAM数据集结果大小、质量和编码时间方面的最佳配置  
- 编写压缩和播放数据集脚本，实现55倍压缩。产出一篇ROBIO论文
- 将Faro 数据集作为真值，编写程序通过对比2个数据集的点云标注动态物体(仍在工作中)
