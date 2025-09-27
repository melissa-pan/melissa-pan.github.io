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
<div class="news-container" id="newsContainer">
{% for item in site.data.news limit:5 %}
<div class="news-item">
<span class="news-date">{{ item.date }}</span>
<span class="news-content">{{ item.content | markdownify | remove: '<p>' | remove: '</p>' | strip }}</span>
</div>
{% endfor %}
{% if site.data.news.size > 5 %}
<div class="news-hidden" style="display: none;">
{% for item in site.data.news offset:5 %}
<div class="news-item">
<span class="news-date">{{ item.date }}</span>
<span class="news-content">{{ item.content | markdownify | remove: '<p>' | remove: '</p>' | strip }}</span>
</div>
{% endfor %}
</div>
{% endif %}
</div>
{% if site.data.news.size > 5 %}
<button class="news-expand-btn" onclick="toggleNews()">Show More News ({{ site.data.news.size | minus: 5 }} more)</button>
{% endif %}
</div>

<script>
function toggleNews() {
  const container = document.getElementById('newsContainer');
  const hiddenNews = document.querySelector('.news-hidden');
  const button = document.querySelector('.news-expand-btn');
  
  if (hiddenNews.style.display === 'none') {
    hiddenNews.style.display = 'block';
    container.classList.remove('collapsed');
    button.textContent = 'Show Less News';
    button.style.background = 'linear-gradient(135deg, #e53e3e 0%, #c53030 100%)';
  } else {
    hiddenNews.style.display = 'none';
    container.classList.add('collapsed');
    button.textContent = 'Show More News ({{ site.data.news.size | minus: 5 }} more)';
    button.style.background = 'linear-gradient(135deg, #667eea 0%, #764ba2 100%)';
  }
}
</script>

---

Hobbies/interests
======
* 🧗‍♀️ I love bouldering: I am a solid V2 climber, my current goal is to climb a V4 route!
* ☕️ My favourite drinks are Iced Americano and Iced Matcha 🍵. I also like making latte art, pattern progress: blob (100%), solid heart (85%), rosetta (20%), ??? (100%).
* 🐶 I love my dog, her name is Paofu. She holds all six level of certifications on behavours and tricks 🎓
* I use emoji exccessively.


Last Update: Dec 2024