---
layout: default
title: Home
---

<section class="hero">
  <div class="hero-content">
    <div class="status-badge">
      <span class="pulse-dot"></span>
      <span class="status-text">Available for New Opportunities</span>
    </div>
    <h1 class="hero-title">Hello, I'm <span class="gradient-text">an Aspiring Developer</span> 👋</h1>
    <p class="hero-desc">I design and build visually stunning, high-performance web applications and love solving algorithmic problems. This is my digital garden for documenting my technical journey, sharing insights, and showcasing my work.</p>
    <div class="social-links">
      <a href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener noreferrer" class="btn btn-primary">
        <i class="fa-brands fa-github"></i> GitHub
      </a>
      <a href="mailto:{{ site.email }}" class="btn btn-outline">
        <i class="fa-solid fa-envelope"></i> Email Me
      </a>
    </div>
  </div>
</section>

<section class="tech-stack-section">
  <h2 class="section-title"><i class="fa-solid fa-layer-group text-gradient-icon"></i> Tech Stack</h2>
  <div class="tech-grid">
    <div class="tech-card">
      <div class="tech-icon"><i class="fa-brands fa-react"></i></div>
      <h3>Frontend</h3>
      <p class="tech-card-desc">Building rich, interactive interfaces with modern frameworks.</p>
      <div class="skills-pills">
        <span>React</span>
        <span>TypeScript</span>
        <span>JavaScript (ES6+)</span>
        <span>HTML5 / CSS3</span>
        <span>TailwindCSS</span>
      </div>
    </div>
    
    <div class="tech-card">
      <div class="tech-icon"><i class="fa-solid fa-server"></i></div>
      <h3>Backend</h3>
      <p class="tech-card-desc">Developing scalable, high-performance APIs and servers.</p>
      <div class="skills-pills">
        <span>Node.js</span>
        <span>Express</span>
        <span>Python</span>
        <span>Django / FastAPI</span>
        <span>RESTful APIs</span>
      </div>
    </div>
    
    <div class="tech-card">
      <div class="tech-icon"><i class="fa-solid fa-screwdriver-wrench"></i></div>
      <h3>Tools & DevOps</h3>
      <p class="tech-card-desc">Managing deployments, versioning, and continuous integration.</p>
      <div class="skills-pills">
        <span>Git & GitHub</span>
        <span>Docker</span>
        <span>PostgreSQL</span>
        <span>AWS</span>
        <span>Vercel / Netlify</span>
      </div>
    </div>
  </div>
</section>

<section class="recent-projects-section">
  <div class="section-header">
    <h2 class="section-title"><i class="fa-solid fa-laptop-code text-gradient-icon"></i> Recent Projects</h2>
    <a href="{{ '/projects/' | relative_url }}" class="view-all-link">View All <i class="fa-solid fa-arrow-right"></i></a>
  </div>
  <div class="project-grid">
    <!-- Project Card 1 -->
    <div class="project-card">
      <div class="project-card-image" style="background-image: linear-gradient(135deg, #1e1b4b 0%, #311042 100%);">
        <div class="project-icon"><i class="fa-solid fa-blog"></i></div>
      </div>
      <div class="project-card-content">
        <div class="project-tags">
          <span>Jekyll</span>
          <span>Liquid</span>
          <span>CSS3</span>
        </div>
        <h3 class="project-title">My Personal Git Blog</h3>
        <p class="project-desc">A premium, high-performance developer portfolio and TIL blog customized with glassmorphism and modern fluid animations.</p>
        <div class="project-links">
          <a href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-github"></i> GitHub</a>
          <a href="#" class="live-demo"><i class="fa-solid fa-globe"></i> Live Demo</a>
        </div>
      </div>
    </div>

    <!-- Project Card 2 -->
    <div class="project-card">
      <div class="project-card-image" style="background-image: linear-gradient(135deg, #022c22 0%, #064e3b 100%);">
        <div class="project-icon"><i class="fa-solid fa-square-poll-vertical"></i></div>
      </div>
      <div class="project-card-content">
        <div class="project-tags">
          <span>React</span>
          <span>Node.js</span>
          <span>MongoDB</span>
        </div>
        <h3 class="project-title">Task Management Dashboard</h3>
        <p class="project-desc">A Kanban-style task management app with multi-workspace support, real-time sync, and rich drag-and-drop interactions.</p>
        <div class="project-links">
          <a href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-github"></i> GitHub</a>
          <a href="#" class="live-demo"><i class="fa-solid fa-globe"></i> Live Demo</a>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="latest-til-section">
  <div class="section-header">
    <h2 class="section-title"><i class="fa-solid fa-book-open text-gradient-icon"></i> Latest TIL</h2>
    <a href="{{ '/til/' | relative_url }}" class="view-all-link">View All <i class="fa-solid fa-arrow-right"></i></a>
  </div>
  
  <div class="til-list">
    {% if site.posts.size > 0 %}
      {% for post in site.posts limit:3 %}
        <a href="{{ post.url | relative_url }}" class="til-card">
          <div class="til-card-left">
            <span class="til-date"><i class="fa-regular fa-calendar"></i> {{ post.date | date: "%b %-d, %Y" }}</span>
            <h3 class="til-title">{{ post.title }}</h3>
          </div>
          <div class="til-card-right">
            <span class="read-more-btn">Read Entry <i class="fa-solid fa-chevron-right"></i></span>
          </div>
        </a>
      {% endfor %}
    {% else %}
      <div class="no-posts-card">
        <i class="fa-regular fa-folder-open icon-empty"></i>
        <h3 class="no-posts-text">No TIL posts published yet.</h3>
        <p class="no-posts-sub">Write markdown files in `_posts` folder to share your learnings!</p>
      </div>
    {% endif %}
  </div>
</section>
