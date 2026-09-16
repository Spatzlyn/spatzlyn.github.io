---
permalink: /
title: "About"
layout: splash
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

{% assign home_avatar = site.author.avatar | default: "profile.png" %}
{% assign home_name = site.author.name | default: site.title %}
{% assign home_email = site.author.email %}
{% assign home_linkedin = site.author.linkedin %}
{% assign home_orcid = site.author.orcid %}
{% assign home_github = site.author.github %}

<div class="home-landing">
  <section class="home-hero" style="--i:0">
    <div class="home-hero__media">
      <div class="home-hero__photo">
        <img class="home-hero__image" src="{{ site.baseurl }}/images/{{ home_avatar }}" alt="{{ home_name }}">
      </div>
      <div class="home-hero__contact">
        <h2>Contact</h2>
        <ul>
          {% if home_email %}
          <li><a href="mailto:{{ home_email }}">{{ home_email }}</a></li>
          {% endif %}
          {% if home_github %}
          <li><a href="https://github.com/{{ home_github }}">GitHub</a></li>
          {% endif %}
          {% if home_linkedin %}
            {% if home_linkedin contains "http" %}
            <li><a href="{{ home_linkedin }}">LinkedIn</a></li>
            {% else %}
            <li><a href="https://{{ home_linkedin }}">LinkedIn</a></li>
            {% endif %}
          {% endif %}
          {% if home_orcid %}
          <li><a href="{{ home_orcid }}">ORCID</a></li>
          {% endif %}
        </ul>
      </div>
    </div>
    <div class="home-hero__content">
      <h1>{{ home_name }}</h1>
      <p>I am an undergraduate student in Computer Science at Korea University. I am interested in how AI systems learn to understand the world — how they perceive, reason, and act in complex environments.</p>
      <p>My research focuses on embodied AI, multimodal learning, and trustworthy AI. I want to build AI that knows when it might be wrong, learns from multiple senses beyond just text, and is reliable enough to actually help people in their everyday lives.</p>
      <p>I care deeply about building AI that is both technically strong and genuinely useful. Pushing the boundaries of what AI can do excites me — but I also believe that technical progress should go hand in hand with thinking about its impact on people. I want to be a researcher who not only advances the field, but also takes responsibility for how their work shapes the world.</p>
      <div class="home-tags">
        <span class="home-tag">Embodied AI</span>
        <span class="home-tag">Multimodal Learning</span>
        <span class="home-tag">Trustworthy AI</span>
        <span class="home-tag">World Models</span>
        <span class="home-tag">AI Reasoning</span>
      </div>
    </div>
  </section>

  <nav class="home-tabs" style="--i:1">
    <a class="home-tabs__link" href="#education">Education</a>
    <a class="home-tabs__link" href="#projects">Projects</a>
    <a class="home-tabs__link" href="#awards">Awards and Honors</a>
    <span class="home-tabs__link is-disabled" aria-disabled="true">CV</span>
  </nav>

  <section id="education" class="home-section" style="--i:2">
    <h2>Education</h2>
    <div class="home-section__card">
      <h3>Korea University - Undergraduate Student <span class="home-section__dates">(23.03~)</span></h3>
      <p>B.S. in Computer Science (in progress)</p>
    </div>
  </section>

  <section id="projects" class="home-section" style="--i:3">
    <h2>Projects</h2>
    <div class="home-section__card">
      <p>Add your research or course projects here. Keep each entry concise with a one-line focus and a link.</p>
    </div>
  </section>

  <section id="awards" class="home-section" style="--i:4">
    <h2>Awards and Honors</h2>
    <div class="home-section__card">
      <ul>
        <li><strong>National Science and Engineering Undergraduate Scholarship</strong> &mdash; Korea Student Aid Foundation &middot; 25.05~</li>
        <li><strong>Samsung Collegiate Programming Challenge 2025 (AI), 1st place</strong> &mdash; Samsung Electronics Co., Ltd. &middot; 25.08 &middot; <a class="home-award__link" href="https://research.samsung.com/news/Samsung-Electronics-Unveils-Winners-of-11th-Collegiate-Programming-Challenge-as-Part-of-AI-Talent-Discovery-Initiative" target="_blank" rel="noopener noreferrer"><i class="fa fa-paperclip" aria-hidden="true"></i> Link</a></li>
      </ul>
    </div>
  </section>
</div>
