---
layout: default
title: Home
---

<div class="home">
  <div class="home-hero">
    <div class="home-hero-inner">
      <div class="home-photo-wrap">
        <img src="{{ '/assets/img/photo.jpg' | relative_url }}" alt="Ankit Mallya" class="home-photo" onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
        <div class="home-photo-placeholder" aria-hidden="true"><span>AM</span></div>
      </div>
      <div class="home-hero-text">
        <h1 class="home-name">{{ site.title }}</h1>
        <p class="home-tagline">Engineering @ BetaNXT</p>
        <p class="home-sub">Engineering → Product · Building products that ship</p>
      </div>
    </div>
  </div>

  <section class="section section-who animate-on-scroll">
    <p class="home-greeting"><span class="greeting-rotate" id="greeting" aria-live="polite">Hello</span>, my name is</p>
    <h2 class="home-intro-line">I build scalable platforms and data systems that ship.</h2>
    <p class="summary-line">Engineering → Product | AWS · Snowflake · dbt | Platform + Data Systems</p>
    <p>
      I'm a software engineer, investor and traveller based in Bangalore, India. I build and ship data pipelines and platform tooling that teams rely on — with a focus on clarity, reliability, and impact.
    </p>
    <p>
      Currently building DataXchange at <a href="https://betanxt.com/" target="_blank" rel="noopener" class="link-highlight">BetaNXT</a>, a fintech company powering wealth management. We're making data flow for advisors and asset managers faster and more reliable.
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

  <section class="section animate-on-scroll">
    <h2>Currently</h2>
    <div class="currently-card">
      <h3>Building DataXchange @ BetaNXT</h3>
      <ul>
        <li>Working on ingestion pipelines and Snowflake/dbt transformations</li>
        <li>Exploring LLM + RAG for enterprise data usability</li>
      </ul>
    </div>
  </section>

  <section class="section animate-on-scroll">
    <h2>Focus areas</h2>
    <div class="focus-grid">
      <div class="focus-card">
        <h3>Technical depth</h3>
        <ul>
          <li>Data pipelines (AWS, Airflow, dbt, Spark)</li>
          <li>Cloud & infra (Terraform, Snowflake, Redshift)</li>
          <li>Schema design, streaming, and governance</li>
        </ul>
      </div>
      <div class="focus-card">
        <h3>Product thinking</h3>
        <ul>
          <li>Problem discovery and prioritization</li>
          <li>Roadmaps and stakeholder alignment</li>
          <li>Metrics and outcome-focused delivery</li>
        </ul>
      </div>
      <div class="focus-card">
        <h3>Execution & collaboration</h3>
        <ul>
          <li>Cross-functional ownership end-to-end</li>
          <li>Specs, reviews, and clear communication</li>
          <li>Shipping on time without sacrificing quality</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="section animate-on-scroll">
    <h2>Quick links</h2>
    <div class="quick-links">
      <a href="{{ '/experience' | relative_url }}" class="pill">Work experience</a>
      <a href="{{ '/blog' | relative_url }}" class="pill">Blog</a>
      <a href="{{ '/cv' | relative_url }}" class="pill">CV</a>
      <a href="https://linkedin.com/in/ankitmallya" class="pill" target="_blank" rel="noopener">LinkedIn</a>
      <a href="mailto:ankit.mallya@gmail.com" class="pill">Email</a>
    </div>
  </section>
</div>
