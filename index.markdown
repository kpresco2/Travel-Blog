---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
<div class="home">
  {%- if page.title -%}
    <h1 class="page-heading">{{ page.title }}</h1>
  {%- endif -%}

  {% for item in site.data.trip_list %}
    <h3>
      <a href="{{ item.link }}">{{ item.name }}</a>
    </h3>
  {% endfor %}
