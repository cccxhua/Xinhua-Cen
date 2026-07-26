---
layout: archive
title: "简历"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

{% assign cv_pdf = "/media/cv/resume.pdf" | prepend: site.baseurl %}

<div style="margin-bottom: 16px;">
  <a href="{{ cv_pdf }}" download="岑欣华-简历.pdf"
     style="display: inline-block; padding: 10px 20px;
            background: #2c7cb0; color: white;
            text-decoration: none; border-radius: 4px;
            font-weight: 500;">
    📥 下载 PDF 简历
  </a>
  <a href="{{ cv_pdf }}" target="_blank"
     style="display: inline-block; padding: 10px 20px;
            background: #6c757d; color: white;
            text-decoration: none; border-radius: 4px;
            font-weight: 500; margin-left: 8px;">
    🔗 新标签页打开
  </a>
</div>

<object data="{{ cv_pdf }}"
        type="application/pdf"
        width="100%" height="900px"
        style="border: 1px solid #ddd; border-radius: 4px;">
  <p style="padding: 20px; background: #f8f9fa; border-radius: 4px;">
    你的浏览器无法直接显示 PDF，请
    <a href="{{ cv_pdf }}">点击这里下载</a>查看。
  </p>
</object>

---

## 更多信息

- 详细教育经历：[/education/]({{ site.baseurl }}/education/)
- 详细实习经历：[/internships/]({{ site.baseurl }}/internships/)
- 详细项目经历：[/projects/]({{ site.baseurl }}/projects/)
