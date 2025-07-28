---
permalink: /
title: "Yinghui He 何映晖"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Hi there! I'm Yinghui He (pronounced as _Yee·ng-Hway Huh_), a second-year PhD student at Princeton University Computer Science Department. I'm honored to be advised by [Sanjeev Arora](https://www.cs.princeton.edu/~arora/) at [Princeton Language and Intelligence](https://pli.princeton.edu/) (PLI). I work in Natural Language Processing, pursuing to develop LLMs and agents to understand the two-way relation between artificial intelligence and human cognition. I finished my Bachelor's degree in Computer Science at the University of Michigan, where I had the honor to work with [Rada Mihalcea](https://web.eecs.umich.edu/~mihalcea/) (at the [LIT Lab](https://lit.eecs.umich.edu/)) and [Wei Hu](https://weihu.me/).

# Publications

{% if site.publication_category %}
{% for category in site.publication_category  %}
{% assign title_shown = false %}
{% for post in site.publications reversed %}
{% if post.category != category[0] %}
{% continue %}
{% endif %}
{% include archive-mainpage.html %}
{% endfor %}
{% endfor %}
{% endif %}
