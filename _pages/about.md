---
permalink: /
title: "Hello there, I'm Aswini Kumar 🙂"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  /* Base Container Styling */
  .about-container {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    line-height: 1.7;
    color: #333;
  }

  /* Typing Effect Intro */
  .typing-container {
    font-size: 1.15em;
    font-weight: 500;
    margin-bottom: 2.5em;
    min-height: 4em;
    color: #2c3e50;
  }
  .cursor {
    display: inline-block;
    width: 3px;
    background-color: #3498db;
    animation: blink 1s step-end infinite;
  }
  @keyframes blink { 50% { opacity: 0; } }

  /* Interactive Cards */
  .interactive-section {
    opacity: 0;
    transform: translateY(20px);
    transition: opacity 0.6s ease-out, transform 0.6s ease-out, box-shadow 0.3s ease;
    margin-bottom: 2em;
    padding: 1.8em;
    border-radius: 12px;
    background: #ffffff;
    border: 1px solid #e1e8ed;
    box-shadow: 0 4px 6px rgba(0,0,0,0.02);
  }
  .interactive-section.visible {
    opacity: 1;
    transform: translateY(0);
  }
  .interactive-section:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.08);
  }

  /* Headings & Links */
  .interactive-section h3 {
    margin-top: 0;
    color: #2c3e50;
    border-bottom: 2px solid #3498db;
    display: inline-block;
    padding-bottom: 4px;
    margin-bottom: 1em;
  }
  a.custom-link {
    color: #3498db;
    text-decoration: none;
    font-weight: 600;
    position: relative;
  }
  a.custom-link::after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 2px;
    bottom: -2px;
    left: 0;
    background-color: #3498db;
    transform-origin: bottom right;
    transition: transform 0.3s ease-out;
  }
  a.custom-link:hover::after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }

  /* Academic Journey Timeline */
  .timeline {
    border-left: 3px solid #3498db;
    padding-left: 20px;
    margin: 10px 0 10px 10px;
  }
  .timeline-item {
    position: relative;
    margin-bottom: 25px;
  }
  .timeline-item:last-child {
    margin-bottom: 0;
  }
  .timeline-item::before {
    content: '';
    position: absolute;
    left: -29px;
    top: 6px;
    width: 12px;
    height: 12px;
    background: #ffffff;
    border: 3px solid #3498db;
    border-radius: 50%;
    transition: background 0.3s, transform 0.3s;
  }
  .timeline-item:hover::before {
    background: #3498db;
    transform: scale(1.3);
  }
  
  /* Flag Counter Image Hover */
  .flag-counter-wrapper img {
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .flag-counter-wrapper img:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 15px rgba(0,0,0,0.15);
  }
</style>

<div class="about-container">
  
  <!-- Animated Intro -->
  <div class="typing-container">
    <span id="typing-text"></span><span class="cursor">&nbsp;</span>
  </div>

  <!-- Current Work Section -->
  <div class="interactive-section">
    <h3>What am I working on now?</h3>
    <p>Currently, I am a final-year doctoral fellow and a <strong>2025 Microsoft PhD Fellow</strong> under the guidance of <a href="https://tanmoychak.com/" class="custom-link" target="_blank">Prof. Tanmoy Chakraborty</a> at the <a href="https://www.lcs2.in/" class="custom-link" target="_blank">Laboratory for Computational Social Systems (LCS2)</a>, IIT Delhi.</p>
    <p>As I work toward my December 2026 thesis synopsis, my research asks a crucial question: <em>How can we detect and mitigate harmful narratives and prevent language models from generating unsafe or damaging responses?</em> My work involves building frameworks like PULSE, exploring mechanistic determinants of model failures, and seeking innovative solutions to make conversational AI more trustworthy and secure.</p>
  </div>

  <!-- Timeline Section -->
  <div class="interactive-section">
    <h3>Where have I come from?</h3>
    <div class="timeline">
      <div class="timeline-item">
        <strong>Research Intern</strong> (Sep - Dec 2025)<br>
        <em>Microsoft Research, Bangalore</em> — Investigated failure aspects and vulnerabilities of LLM agents.
      </div>
      <div class="timeline-item">
        <strong>M.Tech</strong><br>
        <em><a href="https://www.iiitm.ac.in/index.php/en/" class="custom-link" target="_blank">ABV Indian Institute of Information Technology, Gwalior</a></em> — Honored with the Best Postgraduate Merit Award by the Hon’ble President of India, Smt. Droupadi Murmu.
      </div>
      <div class="timeline-item">
        <strong>B.Tech</strong><br>
        <em><a href="https://www.vssut.ac.in/" class="custom-link" target="_blank">Veer Surendra Sai University of Technology, Burla</a></em>.
      </div>
    </div>
  </div>

  <!-- Future Section -->
  <div class="interactive-section">
    <h3>What’s next?</h3>
    <p>In August 2026, I will be joining the <strong>University of Minnesota as a visiting researcher</strong> to expand my work on AI safety and vulnerabilities. I am continually eager to collaborate, review for high-tier academic venues like EMNLP, and contribute to the evolving landscape of language technologies.</p>
  </div>

  <!-- Flag Counter -->
  <div class="flag-counter-wrapper" style="text-align: center; margin-top: 40px;">
    <a href="https://info.flagcounter.com/1dGf" target="_blank">
      <img src="https://s01.flagcounter.com/count2/1dGf/bg_FFFFFF/txt_000000/border_CC0808/columns_4/maxflags_20/viewers_0/labels_0/pageviews_0/flags_0/percent_0/" alt="Flag Counter" border="0">
    </a>
  </div>

</div>

<script>
  // Typing Effect Logic
  const text = "I am a computer science researcher passionate about developing robust large language models (LLMs) and exploring the exciting potential of Diffusion Language Models. My curiosity drives me to push the boundaries of what AI can safely and reliably achieve.";
  const speed = 25; // Speed of typing in ms
  let i = 0;

  function typeWriter() {
    if (i < text.length) {
      document.getElementById("typing-text").innerHTML += text.charAt(i);
      i++;
      setTimeout(typeWriter, speed);
    }
  }

  // Intersection Observer for Scroll Fade-ins
  document.addEventListener("DOMContentLoaded", () => {
    // Start typing effect on load
    typeWriter();

    // Trigger animations when elements scroll into view
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        }
      });
    }, { threshold: 0.15 }); // Triggers when 15% of the element is visible

    document.querySelectorAll('.interactive-section').forEach((section) => {
      observer.observe(section);
    });
  });
</script>
