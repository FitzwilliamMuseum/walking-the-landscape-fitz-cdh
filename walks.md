---
layout: default
title: Walking in Constable's footsteps
permalink: /walks/
---
<section class="mw10 center">

{% for post in site.walks %}
 <article class="pv4  ph3 ph0-l">
      <div class="flex flex-column flex-row-ns">
        <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
          <a href="{{site.baseurl}}{{ post.url }}" title="Read about {{ post.title }}">
            <h1 class="f3 avenir mt0 lh-title">
              {{ post.title }}
            </h1>
          </a>
          <p class="f5 fw4 f4-l lh-copy avenir">
              {{ post.excerpt }}
          </p>
        </div>
        <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
          <img src="{{ post.preview }}" class="db" alt="{{ post.alt_text }}">
        </div>
      </div>
      <p class="f6 lh-copy black mv0">By <span class="text-ink">{{ post.author }}</span></p>
      <time class="f6 db berry">{{ post.date | date: "%A, %b %d %Y" }}</time>
    </article>
{% endfor %}
</section>
