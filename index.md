---
layout: home
title: "Home"
---

<div class="container">
  <header class="text-center">
    <img src="/assets/img/main.jpg" alt="Profile" class="profile-pic">
    <h1>Hey, I'm Walid 👋</h1>
    <p>
      I'm the founder of <a href="https://itsbetter.app" target="_blank">Better</a>, a telehealth startup that aims to help 10,000,000 men in the Middle East with their personal health. I also previously founded <a href="https://callmi.com" target="_blank">Callmi</a>, a platform that lets you book MENA's most in-demand startup experts over a 1:1 video call, as well as <a href="https://addenda.co" target="_blank">Addenda</a>, a blockchain B2B InsurTech, and <a href="https://hala.insure" target="_blank">Hala Insurance</a>, a B2C InsurTech.
    </p>
  </header>
  <section class="links">
    <a href="https://itsbetter.app" class="btn" target="_blank">Better</a>
    <a href="https://callmi.com" class="btn" target="_blank">Callmi</a>
    <a href="https://linkedin.com/in/wdanieldib" class="btn" target="_blank">LinkedIn</a>
  </section>
  <section class="blog-posts">
    <h2>Sometimes I Write Stuff</h2>
    {% for post in site.posts limit: 3 %}
      <div class="post">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p>{{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    {% endfor %}
    <a href="/blog" class="btn">More posts</a>
  </section>
</div>