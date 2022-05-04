---
layout: default
title: Our project team
permalink: /team
---
<section class="mw10 center">
{% for member in site.team %}

<article class="pv4 bb b--black-10 ph3 ph0-l">
<div class="flex flex-column flex-row-ns">
  <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
    <a href="{{ member.url }}"><h1 class="f3 avenir mt0 lh-title">
      {{ member.title }}
    </h1></a>
    <h2 class="f6 fw4 mv0 black-60">Affiliate to: {{ member.institution }}</h2>
    <p class="f5 f4-l fw4  lh-copy avenir">
      {{ member.content | strip_html | truncate: 200 }}
    </p>
  </div>
  <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
    <img src="{{ member.image }}" class="db" alt="A profile photo of {{ member.title }}">
  </div>
</div>
</article>


{% endfor %}
</section>