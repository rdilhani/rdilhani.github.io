---
layout: default
title: "Y M R Dilhani Wepathana"
---
<!-- Hero / Profile -->
<section class="hero" style="text-align:center; padding:2rem 1rem;">
 <img class="profile-photo" src="https://github.com/rdilhani.png" alt="Profile photo"> 
  <h1>Y M R Dilhani Wepathana</h1>
  <p>Workshops • ICT in Education • Educational Technology</p>
</section>

<!-- Slider (Swiper) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.css" />
<section class="home-slider" style="max-width:980px;margin:0 auto;padding:1rem;">
  <div class="swiper" >
    <div class="swiper-wrapper">
      <div class="swiper-slide">
        <img src="/assets/images/slide1.jpg" alt="slide1" style="width:100%;height:360px;object-fit:cover;">
        <div class="slide-caption"><h3>ICT Workshops — Practical Sessions</h3></div>
      </div>
      <div class="swiper-slide">
        <img src="/assets/images/slide2.jpg" alt="slide2" style="width:100%;height:360px;object-fit:cover;">
        <div class="slide-caption"><h3>Online Tools & Classroom Integration</h3></div>
      </div>
      <div class="swiper-slide">
        <img src="/assets/images/slide3.jpg" alt="slide3" style="width:100%;height:360px;object-fit:cover;">
        <div class="slide-caption"><h3>Student-Centered Activities</h3></div>
      </div>
    </div>

    <!-- controls -->
    <div class="swiper-button-prev"></div>
    <div class="swiper-button-next"></div>
    <div class="swiper-pagination"></div>
  </div>
</section>

<!-- Basic profile sections -->
<section style="max-width:980px;margin:1.5rem auto;padding:0 1rem;">
  <h2>About me</h2>
  <p>Short biography — your background, interests, and what you teach/do.</p>

  <h2>Contact</h2>
  <ul>
    <li>Email: rdilhaniw@mail.com</li>
    <li>LinkedIn: <a href="https://www.linkedin.com/in/rdilhani">rdilhani</a></li>
  </ul>
</section>

<!-- Swiper JS -->
<script src="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    const swiper = new Swiper('.swiper', {
      loop: true,
      autoplay: { delay: 4000, disableOnInteraction: false },
      pagination: { el: '.swiper-pagination', clickable: true },
      navigation: { nextEl: '.swiper-button-next', prevEl: '.swiper-button-prev' },
    });
  });
</script>
