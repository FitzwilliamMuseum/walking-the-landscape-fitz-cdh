---
layout: default
title: Our project team
permalink: /team
---
{% for member in site.team %}
<section class="mw10 center">
<article class="pv4 bb b--black-10 ph3 ph0-l">
<div class="flex flex-column flex-row-ns">
  <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
    <h1 class="f3 athelas mt0 lh-title">
      {{ member.title }}
    </h1>
    <p class="f5 f4-l lh-copy athelas">
      Archaeologists have found more than 40 tons of vinyl records,
      some more than a five years old, shedding light on early hipster
      trends.
    </p>
  </div>
  <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
    <img src="http://mrmrs.github.io/photos/warehouse.jpg" class="db" alt="Photo of a warehouse with stacked shelves.">
  </div>
</div>
<p class="f6 lh-copy gray mv0">By <span class="ttu">Imelda Clancy</span></p>
<time class="f6 db gray">Nov. 19, 2016</time>
</article>
</section>

{% endfor %}
