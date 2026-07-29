---
permalink: /internships/
title: "实习经历"
author_profile: true
---

3 段与**强化学习运动控制**方向相关的实习经历。

<!--
======================================================================
🎬 关于视频演示的说明：
- 本地预览（`docker compose up`）时会显示 mp4 视频
- 部署到 GitHub Pages 时只显示 gif（因为 mp4 已被 .gitignore 屏蔽）
- 竖屏 GIF 用固定像素宽度（约 220px）呈现，避免比例过大
- 单独居中的 GIF（乒乓球、动作重定向）用 max-width 520px
======================================================================
-->

---

## 实习 1：桥介数物（深圳）科技有限公司-强化学习算法实习生 软件部


- **技术栈**：Python、PyTorch、Isaac Gym / Isaac Lab、MuJoCo、Gazebo、ROS、URDF / MJCF、PPO

### 核心目标

主要负责足式机器人（四足 + 人形）**运动控制算法架构选型与深度优化**，端到端打通"仿真训练 → 真机部署"的完整链路。

- 参与强化学习算法的**研发与深度优化**，适配连续动作空间
- **分层奖励函数**设计：任务跟踪项（速度 / 姿态）、能耗与力矩正则、动作平滑约束、姿态与关节限位惩罚
- 针对训练建立系统排查流程：
  - **摔倒**：初始位姿随机化 + termination reward 权重调优 + 姿态限位约束
  - **不收敛**：reward 归一化 + entropy schedule + 观测归一化对齐
  - **仿真-真机差异大**：系统辨识 + 域随机化 

### 训练过程

**仿真环境搭建**

- 优化 URDF 机器人模型：碰撞几何简化、惯量与质心校准、传动比与关节限位设定
- 校准物理参数（摩擦系数、armature、joint damping）并添加均匀 / 高斯噪声完成**域随机化**
- 真机环境准备：硬件自检（编码器零位、电机阶跃响应）→ 配置 ROS 通信 → 设置**安全防护层**（力矩上限、姿态阈值触发急停）
- 熟练使用 **Isaac Gym / Isaac Lab / MuJoCo / Gazebo** 四款仿真器，跨平台交叉验证
- 完成仿真与真机环境搭建及验证，无穿模、卡顿、通信延迟超标等问题

**强化学习训练**

- 课程学习：命令幅度由小到大、地形难度阶梯递进
- 实现四足 / 人形机器人**稳定行走、盲爬楼梯**


<div style="display: flex; gap: 12px; flex-wrap: wrap; margin: 16px 0;">
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>仿真</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern1-smallrun-sim.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern1-smallrun-sim.gif"
         alt="小跑步态-仿真" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>实机</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern1-smallrun.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern1-smallrun.gif"
         alt="小跑步态-实机" style="width: 100%;">
    {% endunless %}
  </div>
</div>


<div style="display: flex; gap: 12px; flex-wrap: wrap; margin: 16px 0;">
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>上楼</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern1-stair.mp4#t=24,27" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern1-upstair.gif"
         alt="楼梯-上楼" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>下楼</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern1-stair.mp4#t=15,18" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern1-downstair.gif"
         alt="楼梯-下楼" style="width: 100%;">
    {% endunless %}
  </div>
</div>


## 实习 2：卧安机器人（深圳）股份有限公司-算法实习生 产品研发部

- **技术栈**：Python、Isaac Lab、URDF / MJCF、域随机化、课程学习、PPO

### 自研机器狗的训练与部署

参与自研机器狗的**开发—训练—部署**全流程：

- **结构合理性评估**：从惯量分布、关节自由度等角度评估硬件设计，与机械团队协同迭代
- **训练框架搭建与调参**：确认基线训练框架，调整关键强化学习细节
- **可迁移性验证**：sim2sim（Isaac Lab ↔ MuJoCo）+ sim2real，排查跨平台策略退化
- **成果**：自研机器狗在**平地、坡度、粗糙地面**等复杂地形稳定行走，抗随机推力扰动

<div style="display: flex; gap: 12px; flex-wrap: wrap; justify-content: center; margin: 16px 0;">
  <div style="width: 220px;">
    <p style="margin: 0 0 6px 0; text-align: center;"><strong>常规行走</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-dog1.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-dog1.gif"
         alt="机器狗-常规行走" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="width: 220px;">
    <p style="margin: 0 0 6px 0; text-align: center;"><strong>抗扰动</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-dogrobunst.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-dogrobunst.gif"
         alt="机器狗-抗扰动" style="width: 100%;">
    {% endunless %}
  </div>
</div>

### 自研双足机器人的训练与部署

基于自研机械臂平台**跨形态改造**为双足机器人：

- **硬件重构**：拆卸上肢模块，重新设计双足腿部构型（自由度选择、关节布置、支撑面几何）
- **建模重建**：URDF / MJCF 模型文件从零重建，校准各关节的**质量、质心、惯量张量、限位等**
- **训练策略**：
  - 选用合适的训练框架并高效完成强化学习运动控制训练
  - 构建**域随机化**，**指令课程学习**
- **验证**：搭建 sim2sim 仿真验证（Isaac Lab → MuJoCo），量化跨仿真器的策略一致性，缩小仿真到真机的实际差距


### 机械臂打乒乓球的强化学习训练

参与自研机械臂**乒乓球对打**的创新任务：

- **仿真场景搭建**：基于 **Isaac Lab** 建模球桌、球拍等刚体的碰撞几何、恢复系数、摩擦材质参数，还原真实台球物理
- **发球随机化策略**：控制**落点分布、初速度**，覆盖多样击球场景，增强训练多样性
- **分层奖励设计**（curriculum-style shaping）：
  1. **追踪**：末端到球轨迹预测点的距离奖励，建立基本追踪能力
  2. **击中**：球拍与球实际接触事件，正向击球奖励
  3. **过网**：球被击回过网并落入对方半场，逐步升高权重
  4. **落点精度**：落点与目标位置误差的 Gaussian shaping，训练精确控制
- 训练出机械臂完成**挥拍击球的端到端运动控制策略**

<div style="max-width: 520px; margin: 16px auto; text-align: center;">
  {% unless jekyll.environment == "production" %}
  <video controls style="width: 100%;">
    <source src="{{ site.baseurl }}/media/internships/intern2-pingpongsim.mp4" type="video/mp4">
  </video>
  {% else %}
  <img src="{{ site.baseurl }}/media/internships/intern2-pingpongsim.gif"
       alt="乒乓球-仿真" style="width: 100%;">
  {% endunless %}
  <p style="margin-top: 10px; font-size: 0.95em;">
    源码：<a href="https://github.com/cccxhua/PPO-pingpong/tree/a1-tabletennis"
              target="_blank" rel="noopener">
      cccxhua/PPO-pingpong · a1-tabletennis
    </a>
  </p>
</div>

---

## 实习 3：智元创新（上海）科技股份有限公司-强化学习算法实习生 中央研发部

- **技术栈**：Python、GMR、AMP、Isaac Lab

### 机器人走跑训练优化

- **运动重定向工具链完善**：部署 **GMR系列优化算法**，把不同骨架比例的人体 mocap 数据**重定向**到人形机器人本体，扩充可训练数据集
- **AMP 训练闭环**：将 retargeted motion 稳定接入 **AMP** 训练，判别器 + 任务奖励并行更新
- **成果**：显著改善**走跑运动的自然度与稳定性**，为后续高层控制任务提供**稳定、高效、鲁棒**的底层运动控制方案


<div style="width: 220px; margin: 16px auto; text-align: center;">
  <p style="margin: 0 0 6px 0;"><strong>走跑步态</strong></p>
  {% unless jekyll.environment == "production" %}
  <video controls style="width: 100%;">
    <source src="{{ site.baseurl }}/media/internships/intern3-walkrun.mp4" type="video/mp4">
  </video>
  {% else %}
  <img src="{{ site.baseurl }}/media/internships/intern3-walkrun.gif"
       alt="走跑步态" style="width: 100%;">
  {% endunless %}
</div>

### Sim2Real 真机数据量化对比与关节响应分析

针对同一型号机器人，系统探索**最合适的 PD 参数配置**：

- **实验设计**：保持相同的环境参数、观测归一化、策略网络与随机种子，仅扫描 kp / kd 组合；在同一台真机上依次部署，录制 rosbag 数据包
- **量化指标**：
  - **关节力矩**：均值 / 峰值 / 饱和帧占比，判定是否**超限（>额定力矩）**
  - **关节位置**：目标跟踪误差 RMS、最大偏差、超调量
  - **关节速度**：加速阶段响应时间、稳态噪声
- **分析产出**：对比多组 kp / kd 下"**力矩不超限、关节不过载**"的可行域，供后续同一电机配置的机器人训练直接复用，减少后续项目调参时间

### 机器人感控一体项目

搭配机器人的 **LiDAR + 双目摄像头**，融合**高程图与图像视觉信息**，构建**感知—控制一体化**系统：

- **感知层**：双目立体估计距离/深度 + 目标物体检测
- **决策层**：将感知输出作为 policy 的额外观测
- **执行层**：底层 RL policy 输出关节动作，上层状态机管理任务切换（导航 / 接近 / 抓取 / 搬运）
- **应用场景**：
  - **自主搬运箱子**：识别→接近→稳定持箱
  - **自主避障 / 跨越障碍**：高程图预测支撑面 → 步态调整 → 避让或抬腿越障
- **意义**：进一步落实机器人**实用化部署**，从"能走"迈向"能完成实际任务"

<div style="width: 220px; margin: 16px auto; text-align: center;">
  <p style="margin: 0 0 6px 0;"><strong>自主搬箱</strong></p>
  {% unless jekyll.environment == "production" %}
  <video controls style="width: 100%;">
    <source src="{{ site.baseurl }}/media/internships/intern3-carrybox.mp4" type="video/mp4">
  </video>
  {% else %}
  <img src="{{ site.baseurl }}/media/internships/intern3-carrybox.gif"
       alt="自主搬箱" style="width: 100%;">
  {% endunless %}
</div>
