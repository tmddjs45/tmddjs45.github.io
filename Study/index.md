---
layout: default
title : "Study"
main: true


---


<ul class="catalogue" style="margin-top:0px; margin-bottom:8px;">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blog == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
