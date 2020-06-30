---
layout: page
title: Product
permalink: /product_management/
---

Stay tuned to read about the following: 

1. My experiences with working in the Venture Capital Industry 
2. How to get into Venture Capital industry without a management degree 
3. Deep insights on different sectors and predictions about the future 
4. How to get into Product Management without any prior experience or a management degree 
5. How to create frameworks and learn anything quickly : Ultralearning 
6. Critiquing products and features of different Indian and Global firms 
7. Random Gyaan 

  {% if site.paginate %}
    {% assign posts = paginator.posts %}
  {% else %}
    {% assign posts = site.posts %}
  {% endif %}

{%- if posts.size > 0 -%}
    {%- if page.list_title -%}
      <h2 class="post-list-heading">{{ page.list_title }}</h2>
    {%- endif -%}
    <ul class="post-list">
      {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      {%- for post in posts -%}
      {% if post.title == 'product_management' %}

      <li>
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {%- endif -%}
      {%- endfor -%}
    </ul>

     {%- endif -%}
