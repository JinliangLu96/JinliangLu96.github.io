---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

1. Jinliang Lu and Jiajun Zhang. Improving Unsupervised Neural Machine Translation via Training Data Self-Correction. In Proceedings of 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024), Accepted.

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
