---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I'm a second-year Ph.D. student at UC Berkeley, advised by Prof. [Matei Zaharia](https://people.eecs.berkeley.edu/~matei/) and affiliated with the [Sky Computing Lab](https://sky.cs.berkeley.edu/). My research focuses on **sustainability as a first-order optimization objective** alongside **efficiency** in large-scale machine learning and data center systems. Broadly, I'm interested in:
1. Machine learning systems  
2. Data center computing  
3. Distributed systems  

Before coming to Berkeley, I completed my Master’s degree at Carnegie Mellon University (CMU), where I was very fortunate to work with Prof. [Akshitha Sriraman](https://users.ece.cmu.edu/~asrirama/). My Master’s research centered on developing sustainable resource management techniques for microservices in hyperscale data centers. 

I graduated from the University of Toronto with a Bachelor’s degree in Computer Engineering. While there, I was advised by Prof. [Steve Mann](https://www.ece.utoronto.ca/people/mann-s/) on wearables for prosopagnosia. In between my academic pursuits, I spent ~3 years as a software engineer at IBM working on Db2 database core engine development, specifically on availability features such as backup, restore, and recovery.

Please feel free reach out for research, collaborations, or a casual chat, especially if you are a junior, disadvantaged, or underrepresented student. The best way to reach me is via email:
**[melissapan]@berkeley.edu**


**CV**: [PDF here](../files/cv_2024.pdf), up to Dec 2024.

---

<div class="news-section">
<h1>News</h1>
<div class="news-container">
{% for item in site.data.news %}
<div class="news-item">
<span class="news-date">{{ item.date }}</span>
<span class="news-content">{{ item.content | markdownify | remove: '<p>' | remove: '</p>' | strip }}</span>
</div>
{% endfor %}
</div>
</div>

---

<div class="research-section">
<h2>Selected Research Projects</h2>
{% for paper in site.data.research %}
<div class="research-item{% if paper.featured %} featured{% endif %}">
  <div class="research-header">
    {% if paper.image %}
    <img src="{{ '/images/' | append: paper.image | relative_url }}" alt="{{ paper.title }}" class="research-image">
    {% endif %}
    <div class="research-content">
      <div class="research-title">
        {% if paper.links.pdf %}
          <a href="{{ paper.links.pdf }}">{{ paper.title }}</a>
        {% else %}
          {{ paper.title }}
        {% endif %}
      </div>
      <div class="research-authors">{{ paper.authors | replace: 'Melissa Pan', '<span class="highlight-name">Melissa Pan</span>' }}</div>
      <div class="research-venue">{{ paper.venue }} {{ paper.year }}</div>
      {% if paper.status %}
        <span class="research-status {{ paper.status | downcase | replace: ' ', '-' }}">{{ paper.status }}</span>
      {% endif %}
      {% if paper.award %}
        <span class="research-award {{ paper.award | downcase | replace: ' ', '-' }}">{{ paper.award }}</span>
      {% endif %}
      {% if paper.description %}
        <div class="research-description">{{ paper.description }}</div>
      {% endif %}
      <div class="research-links">
        {% if paper.links.pdf %}
          <a href="{{ paper.links.pdf }}" class="research-link">PDF</a>
        {% endif %}
        {% if paper.links.arxiv %}
          <a href="{{ paper.links.arxiv }}" class="research-link">arXiv</a>
        {% endif %}
        {% if paper.links.code %}
          <a href="{{ paper.links.code }}" class="research-link">Code</a>
        {% endif %}
        {% if paper.links.website %}
          <a href="{{ paper.links.website }}" class="research-link">Website</a>
        {% endif %}
        {% if paper.links.slides %}
          <a href="{{ paper.links.slides }}" class="research-link">Slides</a>
        {% endif %}
        {% if paper.links.poster %}
          <a href="{{ paper.links.poster }}" class="research-link">Poster</a>
        {% endif %}
        {% if paper.links.video %}
          <a href="{{ paper.links.video }}" class="research-link">Video</a>
        {% endif %}
      </div>
    </div>
  </div>
</div>
{% endfor %}
</div>

---

## Teaching & Mentorship & Services

I'm passionate about education and supporting the next generation of (computer) scientists, especially students from underrepresented backgrounds.

**Teaching:**
* **EY: Introduction to Programing Workshop** (Spring 2025) - Designed and lead a 1-day workshop for girls in the area from grade 5 - 9.
* Invited by Dr. [Brad Bass](https://www.environment.utoronto.ca/people/directories/all-faculty/brad-bass) as Guest lectures on sustainable computing and ML systems for University of Toronto's course [ENV360](https://artsci.calendar.utoronto.ca/course/env360h1).
* **18-847: Data Center Computing** (Spring 2024) - Graduate Teaching Assistant at Carnegie Mellon University
* **18-847: Data Center Computing** (Fall 2023) - Graduate Teaching Assistant at Carnegie Mellon University  
* **STEM4Girls Program** - Volunteer mentor for middle school girls interested in STEM

**Mentorship:**
* Berkeley EAAA (2025): PhD application mentoring for underrepresented students
* Berkeley EAAA (2024): PhD application mentoring for underrepresented students
* Regular undergraduate research coffee chats (2024)
* CMU ECE Graduate Mentorship Committee Chair (2024)

**Academic Services:**
* OSDI and ATC 2025 Artifact Evaluation Committee

**Other Services:**
* Berkeley Faculty Hiring Student Committee Chair, EECS Graduate Student Assembly, EECS Grads Matter Committee Member (2025)
* Berkeley Programing System Seminar (PS2) Organizer, Summer Edition on Research Agents (2025)
* Berkeley Graduate Woman of Engineering, Career and Professional Develoment Committee (2024, 2025)
* Berkeley [CSGE](https://csge.berkeley.edu/) Seminar Chair (2024, 2025)
* Berkeley Faculty Hiring Student Committee Member (2024)


---

Hobbies/interests
======
* 🧗‍♀️ I love bouldering: I am a solid V2 climber, my current goal is to climb a V5 route!
* ☕️ My favourite drinks are Iced Americano and Iced Matcha 🍵. I also like making latte art, pattern progress: blob (100%), solid heart (85%), rosetta (20%), ??? (100%).
* 🐶 I love my dog, her name is Paofu. She holds all six level of certifications on behavours and tricks 🎓
* I use emoji exccessively.


This website is last updated: Sep 2025

---

<div style="text-align: center; margin-top: 2rem; padding: 1rem; color: #666; font-size: 0.9rem;">
<p>Visits since my PhD:</p>
<img src="https://visitor-badge.laobi.icu/badge?page_id=melissa-pan.github.io" alt="visitor count" style="display: inline-block;">
</div>