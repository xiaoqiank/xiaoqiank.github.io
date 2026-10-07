---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
publication_order:
  - "10.1109/SP63933.2026.00133"
  - "10.1109/TDSC.2026.3692543"
  - "10.1109/TPDS.2022.3167434"
---

<div class="academic-home">
  <p>I am <strong>Xiaoqian Sun</strong>, a Ph.D. candidate in <strong>Network and Information Security</strong> at the <strong>College of Cryptology and Cyber Science, Nankai University</strong>.</p>
  <p>My research focuses on encrypted database security, searchable encryption, leakage-abuse attacks, and database security.</p>

  <h2>Education</h2>
  <p class="home-education"><strong>Nankai University</strong><br>
  College of Cryptology and Cyber Science<br>
  Ph.D. Candidate in Network and Information Security<br>
  <span class="home-education-date">2023.09–Present</span></p>

  <section id="publications" class="home-publications" aria-labelledby="publications-heading">
    <h2 id="publications-heading">Publications</h2>
    {% for doi in page.publication_order %}
    {% assign paper = site.publications | where: "doi", doi | first %}
    {% if paper %}
    <article class="home-publication">
      <h3>{{ paper.title | escape }}</h3>
      <div class="home-publication-authors">{{ paper.authors | markdownify }}</div>
      <p class="home-publication-venue"><em>{{ paper.venue | escape }}</em>, {{ paper.year }}{% if paper.volume %}, {{ paper.volume }}({{ paper.issue }}){% endif %}, pp. {{ paper.pages }}.</p>
      <p class="home-publication-doi"><a href="https://doi.org/{{ paper.doi }}">DOI: {{ paper.doi }}</a></p>
      <details class="home-publication-abstract">
        <summary>Abstract</summary>
        <div>{{ paper.content | markdownify }}</div>
      </details>
    </article>
    {% endif %}
    {% endfor %}
  </section>
</div>
