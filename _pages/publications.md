---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
---


You can find a comprehensive list of my articles on my [Google Scholar](https://scholar.google.com/citations?user=fV83bm8AAAAJ&hl=en&oi=ao)

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
