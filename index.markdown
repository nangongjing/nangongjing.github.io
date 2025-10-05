---
layout: default
title: "首页"
---

## 欢迎来到我的网站！

这里是我的个人空间，分享技术笔记和生活感悟。

### 最新文章

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})** - {{ post.date | date: "%Y年%m月%d日" }}  
  {{ post.excerpt | strip_html | truncatewords: 20 }}
{% endfor %}

---

[关于我](/about) | [联系我](mailto:your-email@example.com)
