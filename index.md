---
layout: default
title: Home
---

<section class="hero">
  <h1>Hello, I'm an Aspiring Developer 👋</h1>
  <p>I build web applications and love solving algorithmic problems. This is my space for sharing what I learn every day.</p>
  <div class="social-links">
    <a href="https://github.com/{{ site.github_username }}">GitHub</a>
  </div>
</section>

<section class="tech-stack">
  <h2>Tech Stack</h2>
  <ul class="skills-list">
    <li>Frontend: React, JavaScript</li>
    <li>Backend: Node.js, Python</li>
    <li>Tools: Git, Docker</li>
  </ul>
</section>

<section class="recent-projects">
  <h2>Recent Projects</h2>
  <div class="project-grid">
    <!-- Projects will be dynamically loaded here later -->
    <p>Check out my <a href="/projects">Projects</a> page for more.</p>
  </div>
</section>

<section class="latest-til">
  <h2>Latest TIL</h2>
  <ul>
    {% for post in site.posts limit:5 %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</section>
