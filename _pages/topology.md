---
layout: page
title: topology
permalink: /topology/
nav: false
nav_order: 2
---

<style>
	.post-header {
		display: none !important;
	}
	.post-list li {
		padding-top: 0 rem !important;
		padding-bottom: 0 rem !important;
	}
        .post-list li h3 {
          margin-bottom: 0.2rem !important;
        }
        .post-list li p {
          margin-bottom: 0 !important;
        }
</style>

<h1 class="post-title">topology</h1>

<br>
<hr>

<div class="post">

  {% comment %} 从 site.topology 集合中取出所有条目，按 date 排序，再反转（最新在前） {% endcomment %}
  {% assign sorted_items = site.topology | sort: "date" | reverse %}

  <ul class="post-list">
    {% comment %} 遍历排序后的条目，循环变量命名为 item {% endcomment %}
    {% for item in sorted_items %}
      <li>
        <div style="display: flex; align-items: center; justify-content: space-between; gap: 1rem;">

          <!-- 左侧：标题 + 日期 -->
          <div>
            <h3 style="font-size: 1.6rem !important; margin-bottom: 0.25rem;">
              <a class="post-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
            </h3>
            <p class="post-meta" style="font-size: 1.3rem !important; margin: 0;">
              {{ item.date | date: "%B %d, %Y" }}
            </p>
          </div>

          <!-- 右侧：小图片 -->
          {% if item.img %}
          <img src="{{ item.img | relative_url }}"
               style="width: 400px; height: 200px; object-fit: cover; flex-shrink: 0;">
          {% endif %}

        </div>
      </li>
    {% endfor %}
  </ul>

</div>