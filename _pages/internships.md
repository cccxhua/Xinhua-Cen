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
- 竖屏 GIF 在这里用固定像素宽度（约 220px）呈现，避免比例过大
- 单独居中的 GIF（乒乓球、动作重定向）用 max-width 520px
======================================================================
-->

---

## 实习 1：待填写

- **公司 / 机构**：
- **时间**：
- **岗位 / 团队**：
- **主要工作**：
  - 待填写
  - 待填写
- **技术栈**：Python、待补充
- **产出**：待填写

### 演示：小跑步态（仿真 vs 实机）

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

### 演示：楼梯任务（上楼 vs 下楼）

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

---

## 实习 2：待填写

- **公司 / 机构**：
- **时间**：
- **岗位 / 团队**：
- **主要工作**：
  - 待填写
- **技术栈**：
- **产出**：

### 演示：机器狗（竖屏，缩小并排展示）

<div style="display: flex; gap: 12px; flex-wrap: wrap; justify-content: center; margin: 16px 0;">
  <div style="width: 220px;">
    <p style="margin: 0 0 6px 0; text-align: center;"><strong>演示 1</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-dog1.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-dog1.gif"
         alt="机器狗-演示1" style="width: 100%;">
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

### 演示：乒乓球（仿真）

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

## 实习 3：待填写

- **公司 / 机构**：
- **时间**：
- **岗位 / 团队**：
- **主要工作**：
  - 待填写
- **技术栈**：
- **产出**：

### 演示：动作重定向

<div style="max-width: 520px; margin: 16px auto; text-align: center;">
  {% unless jekyll.environment == "production" %}
  <video controls style="width: 100%;">
    <source src="{{ site.baseurl }}/media/internships/intern3-retarget.mp4" type="video/mp4">
  </video>
  {% else %}
  <img src="{{ site.baseurl }}/media/internships/intern3-retarget.gif"
       alt="动作重定向" style="width: 100%;">
  {% endunless %}
</div>

### 演示：搬箱 & 走跑步态（竖屏，缩小并排展示）

<div style="display: flex; gap: 12px; flex-wrap: wrap; justify-content: center; margin: 16px 0;">
  <div style="width: 220px;">
    <p style="margin: 0 0 6px 0; text-align: center;"><strong>搬箱</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern3-carrybox.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern3-carrybox.gif"
         alt="搬箱" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="width: 220px;">
    <p style="margin: 0 0 6px 0; text-align: center;"><strong>走跑步态</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern3-walkrun.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern3-walkrun.gif"
         alt="走跑步态" style="width: 100%;">
    {% endunless %}
  </div>
</div>
