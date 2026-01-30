---
layout: home
title: "Y M R Dilhani Wepathana"
description: "Workshops • ICT in Education • Educational Technology"
---

<div class="profile-grid">
  <!-- Sidebar -->
  <aside class="sidebar-card">
    <img class="profile-photo" src="https://github.com/rdilhani.png" alt="Profile photo"> 
    <div class="name">Y M R Dilhani Wepathana</div>
    <div class="role">ICT Educator • Workshop Facilitator</div>

    <h4>Contact</h4>
    <ul>
      <li><a href="mailto:rdilhaniw@mail.com">rdilhaniw@mail.com</a></li>
      <li><a href="https://www.linkedin.com/in/rdilhani" target="_blank" rel="noopener">LinkedIn</a></li>
    </ul>

    <h4>Quick links</h4>
    <ul>
      <li><a href="{{ '/workshops/' | relative_url }}">Workshops</a></li>
      <li><a href="{{ '/projects/' | relative_url }}">Projects</a></li>
      <li><a href="{{ '/contact/' | relative_url }}">Contact</a></li>
    </ul>

    <h4>Skills</h4>
    <p class="muted">Educational Technology • Instructional Design • Online Tools • Assessment</p>
  </aside>

  <!-- Main column -->
  <div>
    <section class="hero">
      <div>
        <h1>Explore the future of learning with practical ICT workshops</h1>
        <p class="muted">Hands-on sessions, easy classroom integration, and teacher-centred activities that bring technology into learning in meaningful ways.</p>
        <p style="margin-top:0.75rem;"><a class="btn" href="{{ '/workshops/' | relative_url }}">View Workshops</a></p>
      </div>
    </section>

    <!-- Slider -->
    <section class="swiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <img src="{{ '/assets/images/slide1.jpg' | relative_url }}" alt="Practical sessions">
          <div class="slide-caption"><strong>Practical sessions</strong> — activities and step-by-step classroom examples.</div>
        </div>

        <div class="swiper-slide">
          <img src="{{ '/assets/images/slide2.jpg' | relative_url }}" alt="Online Tools">
          <div class="slide-caption"><strong>Online tools</strong> — integrating cloud tools and LMS effectively.</div>
        </div>

        <div class="swiper-slide">
          <img src="{{ '/assets/images/slide3.jpg' | relative_url }}" alt="Assessment">
          <div class="slide-caption"><strong>Assessment & Feedback</strong> — practical techniques for formative assessment.</div>
        </div>
      </div>

      <!-- controls -->
      <div class="swiper-pagination"></div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </section>

    <div class="card">
      <h3>About my workshops</h3>
      <p>My workshops focus on making technology approachable and classroom-ready. They are hands-on and practical, aimed at teachers and educational leaders who want to bring digital tools into their classrooms confidently.</p>
      <p><a href="{{ '/workshops/' | relative_url }}">See full workshop list &rarr;</a></p>
    </div>

    <!-- Recent workshops (auto-list posts tagged 'workshop') -->
    <div class="card" style="margin-top:1rem;">
      <h3>Recent workshops</h3>

      {% assign workshop_posts = site.posts | where_exp:"post","post.tags contains 'workshop'" %}
      {% if workshop_posts.size == 0 %}
        <p class="muted">No workshop posts found yet. Tag posts with <code>workshop</code> to have them listed here.</p>
      {% else %}
        <ul style="margin:0;padding-left:1rem;">
          {% for post in workshop_posts limit:5 %}
            <li style="margin-bottom:0.6rem;">
              <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
              <span class="muted" style="margin-left:0.5rem;font-size:0.95rem;">— {{ post.date | date: "%Y-%m-%d" }}</span>
              {% if post.excerpt %}<div class="muted" style="margin-top:0.25rem;">{{ post.excerpt | strip_html | truncate: 140 }}</div>{% endif %}
            </li>
          {% endfor %}
        </ul>

        <p style="margin-top:0.75rem;"><a href="{{ '/workshops/' | relative_url }}">See all workshops &rarr;</a></p>
      {% endif %}
    </div>

  </div>
</div>
