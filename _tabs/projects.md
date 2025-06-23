---
layout: page
title: Projects
permalink: /projects/
order: 3
---

<style>
  .project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
  }

  .project-card {
    border: 1px solid #ddd;
    border-radius: 10px;
    padding: 15px;
    background-color: #f9f9f9;
    text-align: center;
    transition: box-shadow 0.3s ease;
  }

  .project-card:hover {
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  }

  .project-card img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    border-radius: 5px;
  }

  .project-card h3 {
    margin: 10px 0 5px;
  }
</style>

<div class="project-grid">
  <div class="project-card">
    <a href="/projects/androrat.md/">
      <img src="assets/img/projects/androrat.PNG" alt="AndroRAT Thumbnail">
      <h3>AndroRAT Deployment</h3>
    </a>
    <p>Reverse Android shell for red-team simulation.</p>
  </div>
</div>
