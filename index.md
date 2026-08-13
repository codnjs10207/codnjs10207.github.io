---
layout: default
title: Home
---

<section class="hero">
  <div class="hero-wrapper">
    <div class="hero-content">
      <div class="status-badge">
        <span class="pulse-dot"></span>
        <span class="status-text">Available for New Opportunities</span>
      </div>
      <p class="hero-point">GOOD CODE IS WORTH MORE THAN GOOD DOCUMENTATION.</p>
      <h1 class="hero-title">이채원</h1>
      <p class="hero-desc">복잡한 문제를 마주하고 그 원리를 깊이 있게 파고들어 해결하는 과정을 즐깁니다.<br>
  단순히 기능을 구현하는 것을 넘어, '왜 이 기술을 써야 하는가'를 끊임없이 질문하며 최적의 로직을 탐구합니다.<br>
  매일의 학습 기록(TIL)을 거름 삼아, 어제보다 더 효율적이고 깔끔한 코드를 작성하는 엔지니어로 성장하고 있습니다.</p>
      <div class="social-links">
        <a href="https://github.com/codnjs10207" target="_blank" rel="noopener noreferrer" class="btn btn-primary">
          <i class="fa-brands fa-github"></i> GitHub
        </a>
        <a href="mailto:{{ site.email }}" class="btn btn-outline">
          <i class="fa-solid fa-envelope"></i> Email Me
        </a>
      </div>
    </div>
    <div class="hero-image">
      <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="이채원 프로필 사진">
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
    <a href="https://velog.io/@codnjs623/posts" target="_blank" rel="noopener noreferrer" class="view-all-link">모든 글 보기 <i class="fa-solid fa-arrow-up-right-from-square"></i></a>
  </div>
  
  <div class="til-card-grid">
    <!-- TIL Card 1 -->
    <div class="til-post-card">
      <div class="til-post-content">
        <div class="til-post-meta">
          <span class="til-post-category"><i class="fa-solid fa-server"></i> 백엔드 • Node.js</span>
          <span class="til-post-date">2026.08.13</span>
        </div>
        <h3 class="til-post-title">Node.js 비동기 처리와 이벤트 루프의 이해</h3>
        <p class="til-post-summary">Node.js의 핵심 구조인 싱글 스레드 논블로킹 I/O 모델과 이를 가능하게 하는 이벤트 루프(Event Loop)의 단계를 깊이 있게 알아봅니다. Call Stack, Callback Queue의 관계와 마이크로태스크 큐의 우선순위를 분석합니다.</p>
      </div>
      <div class="til-post-footer">
        <a href="https://velog.io/@codnjs623/posts" target="_blank" rel="noopener noreferrer" class="til-read-btn">
          글 읽기 <i class="fa-solid fa-arrow-right"></i>
        </a>
      </div>
    </div>

    <!-- TIL Card 2 -->
    <div class="til-post-card">
      <div class="til-post-content">
        <div class="til-post-meta">
          <span class="til-post-category"><i class="fa-solid fa-laptop-code"></i> 프론트엔드 • React</span>
          <span class="til-post-date">2026.08.12</span>
        </div>
        <h3 class="til-post-title">React 19 Server Components와 데이터 페칭 최적화</h3>
        <p class="til-post-summary">React 19에서 정식 도입된 React Server Components(RSC)의 동작 원리를 파헤칩니다. 클라이언트 컴포넌트와의 경계를 설계하고, 서버단 데이터 페칭과 Suspense를 활용하여 번들 사이즈와 로딩 타임을 비약적으로 절감하는 기법을 소개합니다.</p>
      </div>
      <div class="til-post-footer">
        <a href="https://velog.io/@codnjs623/posts" target="_blank" rel="noopener noreferrer" class="til-read-btn">
          글 읽기 <i class="fa-solid fa-arrow-right"></i>
        </a>
      </div>
    </div>
  </div>
</section>
