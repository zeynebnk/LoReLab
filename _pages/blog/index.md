---
layout: page
title: News
permalink: /news/
toggle: on
rank: 1
---

<ul class="post-list">
    {% for post in site.posts %}
      <li>
        <p style="font-size:20px;">
        <b>

         {{ post.date | date: "%b %-d, %Y" | append: " ––"}} </b> {{ post.title }} </p>
    
        <p>
         {{ post.excerpt}}
        </p>
      </li>
    {% endfor %}
  </ul>