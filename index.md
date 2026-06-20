---
layout: homepage
title: Home
---

<section class="content-block" id="bio">
  <div class="section-heading">
    <span class="section-icon" aria-hidden="true"><i class="fas fa-user"></i></span>
    <h2>Biography</h2>
  </div>
  <p>
    I am a postdoctoral researcher at <a href="https://en.westlake.edu.cn/">Westlake University</a>, working with
    <a href="https://scholar.google.com/citations?hl=en&amp;user=vAIECxgAAAAJ">Prof. Yefeng Zheng</a> (IEEE &amp; AIMBE Fellow).
    I received my Ph.D. degree from <a href="https://www.isct.ac.jp/en">Science Tokyo</a>. Before that, I obtained my M.Sc.
    from <a href="https://hkust.edu.hk/">Hong Kong University of Science and Technology</a> and my bachelor's degree from
    <a href="https://www.whut.edu.cn/">Wuhan University of Technology</a>.
  </p>
</section>

<section class="content-block" id="research-interests">
  <div class="section-heading">
    <span class="section-icon" aria-hidden="true"><i class="fas fa-lightbulb"></i></span>
    <h2>Research Interests</h2>
  </div>
  <p>
    I build <strong>Trustworthy Medical AI</strong> systems designed for the complexities of real-world clinical
    deployment. By addressing core challenges in model robustness, privacy preservation, and lifecycle safety, my
    research aims to develop dependable tools that responsibly integrate into dynamic healthcare environments.
  </p>
  <div class="interest-hierarchy">
    <div class="interest-theme">
      <span>Research Direction</span>
      <strong>Trustworthy Medical AI</strong>
    </div>
    <div class="interest-grid" aria-label="Subareas of Trustworthy Medical AI">
      <article>
        <h3>Robustness &amp; Generalization</h3>
        <p>Domain generalization, test-time adaptation, and semi-supervised learning for reliable medical image and signal processing.</p>
      </article>
      <article>
        <h3>Privacy Preservation</h3>
        <p>Federated learning, machine unlearning, and data-use rights protection via unlearnable examples for sensitive clinical data.</p>
      </article>
      <article>
        <h3>Lifecycle Medical AI</h3>
        <p>Continuous validation, deployment-time monitoring, and dynamic updates across the lifespan of medical AI systems.</p>
      </article>
      <article>
        <h3>Safety &amp; Evaluation</h3>
        <p>Safety alignment and rigorous evaluation for medical foundation models, including VLMs and autonomous clinical agents.</p>
      </article>
    </div>
  </div>
</section>

<section class="content-block" id="news">
  <div class="section-heading">
    <span class="section-icon" aria-hidden="true"><i class="fas fa-bullhorn"></i></span>
    <h2>News</h2>
  </div>
  <ul class="news-list">
    <li>
      <time>May 2026</time>
      <p>Two papers were accepted to MICCAI 2026: VoxShield and BeatRhythm-TTA.</p>
    </li>
    <li>
      <time>Apr 2026</time>
      <p>Our paper "FedSemiDG: Domain Generalized Federated Semi-supervised Medical Image Segmentation" was accepted by Medical Image Analysis.</p>
    </li>
    <li>
      <time>Mar 2025</time>
      <p>I passed the final defense of my Ph.D. thesis and graduated from Science Tokyo.</p>
    </li>
    <li>
      <time>Sep 2024</time>
      <p>Our contributed book chapter on federated learning in modern medical imaging was published.</p>
    </li>
  </ul>
  <a class="text-link" href="{{ '/news.html' | relative_url }}">More news <span aria-hidden="true">&rarr;</span></a>
</section>

<section class="content-block" id="selected-publications">
  <div class="section-heading">
    <span class="section-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
    <h2>Selected Publications</h2>
  </div>
  {% include selected-publications.md %}
  <a class="text-link" href="{{ '/publications.html' | relative_url }}">View all publications <span aria-hidden="true">&rarr;</span></a>
</section>
