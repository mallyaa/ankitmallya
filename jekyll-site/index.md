---
layout: default
title: Home
---

<div class="home">
  <div class="home-hero">
    <div class="home-photo-wrap">
      <img src="{{ '/assets/img/photo.jpg' | relative_url }}" alt="Ankit Mallya" class="home-photo" onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
      <div class="home-photo-placeholder" aria-hidden="true"><span>AM</span></div>
    </div>
    <h1 class="home-name">{{ site.title }}</h1>
    <p class="home-tagline">Tech Product Manager</p>
    <p class="home-sub">Engineering → Product · Building products that ship</p>
  </div>

  <section class="section section-who">
    <p class="home-greeting"><span class="greeting-rotate" id="greeting" aria-live="polite">Hello</span>, my name is</p>
    <h2 class="home-intro-line">I enjoy building things.</h2>
    <p>
      I'm a software engineer, investor and traveler currently based in Bangalore, India.
    </p>
    <p>
      Currently building DataXchange for <a href="https://betanxt.com/" target="_blank" rel="noopener" class="link-highlight">BetaNXT</a> — a fintech company powering wealth management; we're making data flow for advisors and asset managers faster and more reliable.
    </p>
    <script>
      (function() {
        var greetings = ['Namaste', 'Bonjour', 'Hello', 'Hola', 'Ciao'];
        var el = document.getElementById('greeting');
        if (!el) return;
        var i = 0;
        setInterval(function() {
          i = (i + 1) % greetings.length;
          el.textContent = greetings[i];
        }, 2200);
      })();
    </script>
  </section>

  <section class="section">
    <h2>Quick links</h2>
    <p>
      <a href="{{ '/experience' | relative_url }}">Work experience</a> ·
      <a href="{{ '/blog' | relative_url }}">Blog</a> ·
      <a href="{{ '/cv' | relative_url }}">CV</a> ·
      <a href="https://linkedin.com/in/ankitmallya" target="_blank" rel="noopener">LinkedIn</a> ·
      <a href="mailto:ankit.mallya@gmail.com">Email</a>
    </p>
  </section>
</div>
