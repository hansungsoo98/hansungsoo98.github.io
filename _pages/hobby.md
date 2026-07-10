---
layout: page
title: hobby
permalink: /hobby/
description: A small collection of things I enjoy outside research.
nav: true
nav_order: 6
---

<style>
  .hobby-page {
    --hobby-accent: #b400b9;
    --hobby-border: rgba(0, 0, 0, 0.1);
  }

  .hobby-intro {
    max-width: 720px;
    margin-bottom: 1.75rem;
  }

  .hobby-intro p {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 1.02rem;
    line-height: 1.7;
  }

  .hobby-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.25rem;
  }

  .hobby-card {
    position: relative;
    overflow: hidden;
    min-height: 320px;
    border: 1px solid var(--hobby-border);
    border-radius: 0.5rem;
    background: #111111;
    isolation: isolate;
  }

  .hobby-card img {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    transform: scale(1.02);
    transition: transform 240ms ease;
    z-index: -2;
  }

  .hobby-card::after {
    content: "";
    position: absolute;
    inset: 0;
    background: linear-gradient(180deg, rgba(0, 0, 0, 0.05) 15%, rgba(0, 0, 0, 0.68) 100%);
    z-index: -1;
  }

  .hobby-card:hover img {
    transform: scale(1.06);
  }

  .hobby-content {
    min-height: 320px;
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    gap: 0.7rem;
    padding: 1.35rem;
    color: #ffffff;
  }

  .hobby-label {
    width: fit-content;
    padding: 0.22rem 0.7rem;
    border-radius: 999px;
    background: var(--hobby-accent);
    color: #ffffff;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0;
    text-transform: uppercase;
  }

  .hobby-card h2 {
    margin: 0;
    color: #ffffff;
    font-size: 1.55rem;
    font-weight: 700;
    letter-spacing: 0;
  }

  .hobby-card p {
    margin: 0;
    max-width: 34rem;
    color: rgba(255, 255, 255, 0.86);
    line-height: 1.55;
  }

  @media (max-width: 768px) {
    .hobby-grid {
      grid-template-columns: 1fr;
      gap: 1rem;
    }

    .hobby-card,
    .hobby-content {
      min-height: 260px;
    }
  }
</style>

<div class="hobby-page">
  <div class="hobby-intro">
    <p>
      A few things I enjoy outside the lab. These are temporary preview images for now, and each card can be swapped with
      personal photos later.
    </p>
  </div>

  <div class="hobby-grid">
    <article class="hobby-card">
      <img src="{{ '/assets/img/3.jpg' | relative_url }}" alt="Badminton preview image">
      <div class="hobby-content">
        <span class="hobby-label">sport</span>
        <h2>Badminton</h2>
        <p>Quick rallies, small adjustments, and the satisfying sound of a clean shot.</p>
      </div>
    </article>

    <article class="hobby-card">
      <img src="{{ '/assets/img/12.jpg' | relative_url }}" alt="Classical guitar preview image">
      <div class="hobby-content">
        <span class="hobby-label">music</span>
        <h2>Classical Guitar</h2>
        <p>Quiet practice time with nylon strings, small details, and pieces that reward patience.</p>
      </div>
    </article>

    <article class="hobby-card">
      <img src="{{ '/assets/img/10.jpg' | relative_url }}" alt="Minesweeper preview image">
      <div class="hobby-content">
        <span class="hobby-label">puzzle</span>
        <h2>Minesweeper</h2>
        <p>A tiny logic game with just enough uncertainty to make every click feel dramatic.</p>
      </div>
    </article>

    <article class="hobby-card">
      <img src="{{ '/assets/img/1.jpg' | relative_url }}" alt="Walking preview image">
      <div class="hobby-content">
        <span class="hobby-label">routine</span>
        <h2>Walking</h2>
        <p>Slow, useful time for sorting thoughts, resetting focus, and letting ideas settle.</p>
      </div>
    </article>

  </div>
</div>
