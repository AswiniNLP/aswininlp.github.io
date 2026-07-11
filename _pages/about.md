---
permalink: /
title: "Hello there, I'm Aswini Kumar 🙂"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  /* Cosmic Background & Base Styling */
  body {
    background: radial-gradient(ellipse at bottom, #1b2735 0%, #090a0f 100%);
    color: #e6edf3;
    margin: 0;
    overflow-x: hidden;
  }

  .about-container {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    line-height: 1.7;
    position: relative;
    z-index: 1;
    padding: 2em;
    max-width: 800px;
    margin: 0 auto;
  }

  /* Animated Planets & Space Elements */
  .space-bg {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    z-index: 0;
    pointer-events: none;
    overflow: hidden;
  }

  .planet {
    position: absolute;
    border-radius: 50%;
    box-shadow: inset -15px -15px 40px rgba(0,0,0,0.5), 0 0 20px rgba(255,255,255,0.1);
  }

  .planet-jupiter {
    width: 120px;
    height: 120px;
    top: 15%;
    right: 10%;
    background: linear-gradient(145deg, #c3a171, #8b5a2b, #d9b88f);
    animation: float 25s ease-in-out infinite;
  }

  /* Orbiting Ring for Jupiter-like planet */
  .planet-jupiter::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 200px;
    height: 60px;
    border: 8px solid rgba(200, 180, 150, 0.4);
    border-radius: 50%;
    transform: translate(-50%, -50%) rotate(20deg);
    box-shadow: 0 0 15px rgba(200, 180, 150, 0.2);
  }

  .planet-mars {
    width: 60px;
    height: 60px;
    bottom: 20%;
    left: 5%;
    background: radial-gradient(circle at 30% 30%, #e74c3c, #96281b);
    animation: float 18s ease-in-out infinite reverse;
  }

  .planet-moon {
    width: 30px;
    height: 30px;
    top: 50%;
    right: 25%;
    background: radial-gradient(circle at 30% 30%, #bdc3c7, #7f8c8d);
    animation: orbit 20s linear infinite;
  }

  /* Keyframes for Space Animations */
  @keyframes float {
    0%, 100% { transform: translateY(0px) rotate(0deg); }
    50% { transform: translateY(-40px) rotate(5deg); }
  }

  @keyframes orbit {
    0% { transform: rotate(0deg) translateX(100px) rotate(0deg); }
    100% { transform: rotate(360deg) translateX(100px) rotate(-360deg); }
  }

  /* Typing Effect Intro */
  .typing-container {
    font-size: 1.15em;
    font-weight: 400;
    margin-bottom: 2.5em;
    min-height: 5em;
    color: #c9d1d9;
    text-shadow: 0 2px 4px rgba(0,0,0,0.5);
  }
  .cursor {
    display: inline-block;
    width: 3px;
    background-color: #58a6ff;
    animation: blink 1s step-end infinite;
  }
  @keyframes blink { 50% { opacity: 0; } }

  /* Glassmorphism Interactive Cards */
  .interactive-section {
    opacity: 0;
    transform: translateY(20px);
    transition: opacity 0.6s ease-out, transform 0.6s ease-out, box-shadow 0.3s ease;
    margin-bottom: 2.5em;
    padding: 2em;
    border-radius: 16px;
    /* Glass effect */
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.3);
  }
  .interactive-section.visible {
    opacity: 1;
    transform: translateY(0);
  }
  .interactive-section:hover {
    transform: translateY(-5px);
    box-shadow: 0 12px 40px 0 rgba(0, 0, 0, 0.5);
    border: 1px solid rgba(88, 166, 255, 0.3);
  }

  /* Headings & Links */
  .interactive-section h3 {
    margin-top: 0;
    color: #ffffff;
    border-bottom: 2px solid #58a6ff;
    display: inline-block;
    padding-bottom: 6px;
    margin-bottom: 1.2em;
    letter-spacing: 0.5px;
  }
  a.custom-link {
    color: #58a6ff;
    text-decoration: none;
    font-weight: 600;
    position: relative;
    transition: color 0.3s;
  }
  a.custom-link::after {
    content: '';
    position: absolute;
    width: 100%;
    transform: scaleX(0);
    height: 2px;
    bottom: -2px;
    left: 0;
    background-color: #58a6ff;
    transform-origin: bottom right;
    transition: transform 0.3s ease-out;
  }
  a.custom-link:hover {
    color: #79c0ff;
  }
  a.custom-link:hover::after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }

  /* Academic Journey Timeline */
  .timeline {
    border-left: 2px solid rgba(88, 166, 255, 0.4);
    padding-left: 25px;
    margin: 15px 0 15px 15px;
  }
  .timeline-item {
    position: relative;
    margin-bottom: 30px;
    color: #c9d1d9;
  }
  .timeline-item:last-child {
    margin-bottom: 0;
  }
  .timeline-item::before {
    content: '';
    position: absolute;
    left: -32px;
    top: 6px;
    width: 10px;
    height: 10px;
    background: #090a0f;
    border: 2px solid #58a6ff;
    border-radius: 50%;
    transition: background 0.3s, transform 0.3s, box-shadow 0.3s;
  }
  .timeline-item:hover::before {
    background: #58a6ff;
    transform: scale(1.4);
    box-shadow: 0 0 10px #58a6ff;
  }
  strong {
    color: #ffffff;
  }

  /* Flag Counter Image Hover */
  .flag-counter-wrapper img {
    border-radius: 8px;
    background: rgba(255,255,255,0.9);
    padding: 5px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.4);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .flag-counter-wrapper img:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 25px rgba(88, 166, 255, 0.3);
  }
</style>

<!-- Background Animation Layer -->
<div class="space-bg">
  <div class="planet planet-jupiter"></div>
  <div class="planet planet-mars"></div>
  <div class="planet planet-moon"></div>
</div>

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
    }, { threshold: 0.15 }); 

    document.querySelectorAll('.interactive-section').forEach((section) => {
      observer.observe(section);
    });
  });
</script>
