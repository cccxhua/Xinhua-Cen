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
- 要在网页上真正显示 GIF，需要把对应的 .gif 文件放到 media/internships/
  （用 ffmpeg 或在线工具从 mp4 生成）
- 文件名建议改成有意义的名字，例如 intern1_walking.mp4 / intern1_walking.gif
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

### 演示：机器狗

<div style="display: flex; gap: 12px; flex-wrap: wrap; margin: 16px 0;">
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>演示 1</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-dog1.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-dog1.gif"
         alt="机器狗-演示1" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>抗扰动</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-dogrobunst.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-dogrobunst.gif"
         alt="机器狗-抗扰动" style="width: 100%;">
    {% endunless %}
  </div>
</div>

### 演示：腿部控制

<div style="display: flex; gap: 12px; flex-wrap: wrap; margin: 16px 0;">
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>演示 1</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-legs1.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-legs1.gif"
         alt="腿部控制-演示1" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="flex: 1; min-width: 280px;">
    <p style="margin: 0 0 6px 0;"><strong>演示 2</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern2-legs2.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern2-legs2.gif"
         alt="腿部控制-演示2" style="width: 100%;">
    {% endunless %}
  </div>
</div>

### 演示：乒乓球（仿真）

<div style="max-width: 50%; min-width: 280px; margin: 16px 0;">
  {% unless jekyll.environment == "production" %}
  <video controls style="width: 100%;">
    <source src="{{ site.baseurl }}/media/internships/intern2-pingpongsim.mp4" type="video/mp4">
  </video>
  {% else %}
  <img src="{{ site.baseurl }}/media/internships/intern2-pingpongsim.gif"
       alt="乒乓球-仿真" style="width: 100%;">
  {% endunless %}
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

### 演示

<div style="display: flex; gap: 12px; flex-wrap: wrap; margin: 16px 0;">
  <div style="flex: 1; min-width: 260px;">
    <p style="margin: 0 0 6px 0;"><strong>搬箱</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern3-carrybox.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern3-carrybox.gif"
         alt="搬箱" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="flex: 1; min-width: 260px;">
    <p style="margin: 0 0 6px 0;"><strong>动作重定向</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern3-retarget.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern3-retarget.gif"
         alt="动作重定向" style="width: 100%;">
    {% endunless %}
  </div>
  <div style="flex: 1; min-width: 260px;">
    <p style="margin: 0 0 6px 0;"><strong>走跑步态</strong></p>
    {% unless jekyll.environment == "production" %}
    <video controls style="width: 100%; max-width: 100%;">
      <source src="{{ site.baseurl }}/media/internships/intern3-walkrun.mp4" type="video/mp4">
    </video>
    {% else %}
    <img src="{{ site.baseurl }}/media/internships/intern3-walkrun.gif"
         alt="走跑步态" style="width: 100%;">
    {% endunless %}
  </div>
</div>

<!--
======================================================================
🔧 添加更多视频的模板（复制粘贴即可）：

{% unless jekyll.environment == "production" %}
<video width="640" controls>
  <source src="{{ site.baseurl }}/media/internships/你的视频名.mp4" type="video/mp4">
</video>
{% else %}
![说明]({{ site.baseurl }}/media/internships/你的视频名.gif)
{% endunless %}
======================================================================
-->
