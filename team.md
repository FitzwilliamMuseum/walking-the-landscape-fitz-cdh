---
layout: default
title: Our project team
permalink: /team/
image: https://data.fitzmuseum.cam.ac.uk/imagestore/portfolio/F25982D9_7CB9_CFFF_028E_8BBFC531887C/588/729/medium_P_1489_R_mas.jpg
---
<section class="mw10 center">
{% for member in site.team %}

<article class="pv4 bb b--black-10 ph3 ph0-l">
<div class="flex flex-column flex-row-ns">
  <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
    <a href="{{ member.url }}"><h1 class="f3 avenir mt0 lh-title">
      {{ member.title }}
    </h1></a>
    <h2 class="f5 fw4 mv0 berry">Affiliated to: {{ member.institution }}</h2>
    <p class="f5 f5-l fw4  lh-copy avenir">
      {{ member.content | strip_html | truncate: 400 }}
    </p>

  </div>
  <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
    <img src="{{ member.image }}" class="db" alt="A profile photo of {{ member.title }}">
  </div>
</div>
</article>


{% endfor %}
</section>