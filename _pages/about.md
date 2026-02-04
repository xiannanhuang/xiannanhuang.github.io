---
permalink: /
title: "Welcome to My Academic Homepage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. candidate in Transportation Engineering at Tongji University, advised by Prof. Chao Yang. My research focuses on **online learning for traffic demand prediction**, **uncertainty quantification**, and **causal inference in urban mobility systems**.

Education
======
* **Ph.D. in Transportation Engineering**, Tongji University, 2022–Present  
* **M.S. in Transportation Engineering**, Tongji University, 2020–2022  
* **B.S. in Civil Engineering**, Tongji University, 2016–2020

My recent work includes:

Publications
======
<ul>
{% for post in site.publications reversed %}
  <li>
    <b>{{ post.title }}</b><br />
    {{ post.authors }}, {{ post.year }}<br />
    {% if post.journal %}
      <i>{{ post.journal }}</i>
    {% elsif post.conference %}
      <i>{{ post.conference }}</i>
    {% elsif post.arxiv %}
      <a href="{{ post.arxiv }}">arXiv preprint</a>
    {% endif %}
    {% if post.doi %}
      | <a href="https://doi.org/{{ post.doi }}">DOI</a>
    {% endif %}
    {% if post.pdf %}
      | <a href="{{ post.pdf | relative_url }}">PDF</a>
    {% endif %}
  </li>
{% endfor %}
</ul>


  
📄 [View my publications](/publications)  
