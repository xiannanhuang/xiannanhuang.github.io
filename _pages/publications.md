---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<ul>
{% for pub in site.publications reversed %}
  <li>
    <b>{{ pub.title }}</b><br />
    {{ pub.authors | default: pub.author }}, {{ pub.year | default: "n.d." }}<br />
    {% if pub.journal %}
      <i>{{ pub.journal }}</i>
    {% elsif pub.conference %}
      <i>{{ pub.conference }}</i>
    {% elsif pub.venue %}
      <i>{{ pub.venue }}</i>
    {% endif %}
    {% if pub.doi %}
      | <a href="https://doi.org/{{ pub.doi }}">DOI</a>
    {% endif %}
    {% if pub.arxiv %}
      | <a href="{{ pub.arxiv }}">arXiv</a>
    {% endif %}
  </li>
{% endfor %}
</ul>
