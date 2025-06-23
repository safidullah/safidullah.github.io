---
layout: page
title: Projects
permalink: /projects/
---

<style>
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 1.5rem;
  margin-top: 1rem;
}

.project-card {
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.2s;
  text-align: center;
  padding: 1rem;
}

.project-card:hover {
  transform: scale(1.03);
}

.project-card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
}

.project-card h3 {
  margin: 0.8rem 0 0.3rem;
}

.project-card p {
  font-size: 0.9rem;
  color: #666;
}
</style>

<div class="project-grid">
  <div class="project-card">
    <a href="{{ '/projects/androrat' | relative_url }}">
      <img src="{{ '/assets/img/projects/androrat.png' | relative_url }}" alt="AndroRAT Project Thumbnail">
      <h3>AndroRAT Deployment</h3>
    </a>
    <p>Reverse Android shell for red-team simulation.</p>
  </div>

  <!-- Add more cards below the same way -->
</div>
