---
layout: about
title: 合作教授
permalink: /
# subtitle: <a href='#'>单位</a>. 地址. 联系方式. 座右铭等.
lang: zh
nav: true
nav_order: 1

# profile:
#   align: right
#   image: prof_pic.jpg
#   image_circular: false # crops the image to make it circular
#   more_info: >
#     <p>555 你的办公室号码</p>
#     <p>123 你的地址街道</p>
#     <p>你的城市, 省份 12345</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
.team-avatar {
  width: 120px;
  height: 120px;
  object-fit: cover;
  margin: 0 auto;
}
.team-name {
  font-size: 1.1em;
  font-weight: bold;
}
.team-role {
  font-size: 0.85em;
}
.section-anchor {
  scroll-margin-top: 80px;
}
.section-title {
  color: #b509ac;
  font-weight: bold;
  margin-top: 2rem;
  margin-bottom: 1.5rem;
}
.team-category-title {
  font-size: 1.3rem;
  font-weight: 600;
  margin-top: 1.5rem;
  margin-bottom: 1rem;
}
@media (min-width: 992px) {
  .col-lg-5ths {
    flex: 0 0 20%;
    max-width: 20%;
  }
}
</style>

<h2 class="section-title">🎓合作教授</h2>

<h3 class="team-category-title">网络技术</h3>

<hr>

<div class="row text-center mb-1 justify-content-center">
{% for member in site.data.team.network_tech %}
  <div class="col-6 col-sm-4 col-md-3 col-lg-5ths mb-4">
    {% if member.url %}
    <a href="{{ member.url | relative_url }}" style="color: inherit; text-decoration: none;">
    {% endif %}
      <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" class="img-fluid rounded-circle z-depth-1 team-avatar" alt="{{ member.name }}">
      <div class="team-name mt-2">{{ member.name }}</div>
      <div class="text-muted team-role">{{ member.role }}</div>
    {% if member.url %}
    </a>
    {% endif %}
  </div>
{% endfor %}
</div>

<h3 class="team-category-title">先进计算</h3>

<hr>

<div class="row text-center mb-1 justify-content-center">
{% for member in site.data.team.advanced_computing %}
  <div class="col-6 col-sm-4 col-md-3 col-lg-5ths mb-4">
    {% if member.url %}
    <a href="{{ member.url | relative_url }}" style="color: inherit; text-decoration: none;">
    {% endif %}
      <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" class="img-fluid rounded-circle z-depth-1 team-avatar" alt="{{ member.name }}">
      <div class="team-name mt-2">{{ member.name }}</div>
      <div class="text-muted team-role">{{ member.role }}</div>
    {% if member.url %}
    </a>
    {% endif %}
  </div>
{% endfor %}
</div>

<h3 class="team-category-title">存储与数据</h3>

<hr>

<div class="row text-center mb-1 justify-content-center">
{% for member in site.data.team.storage_data %}
  <div class="col-6 col-sm-4 col-md-3 col-lg-5ths mb-4">
    {% if member.url %}
    <a href="{{ member.url | relative_url }}" style="color: inherit; text-decoration: none;">
    {% endif %}
      <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" class="img-fluid rounded-circle z-depth-1 team-avatar" alt="{{ member.name }}">
      <div class="team-name mt-2">{{ member.name }}</div>
      <div class="text-muted team-role">{{ member.role }}</div>
    {% if member.url %}
    </a>
    {% endif %}
  </div>
{% endfor %}
</div>
