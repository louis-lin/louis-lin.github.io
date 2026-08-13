---
layout: page
title: Photos
permalink: /photos/
nav: true
nav_order: 5
description: Lab and field work, plus the occasional non-research photo.
---

<!-- Before adding lab/research photos here, run them through the media clearance
     checklist in EDITORIAL.md / the build spec (section 6): already published with
     rights retained? sponsor/PI clearance for proprietary or unpublished content?
     consent from anyone identifiable in the photo? -->

## Research

<div class="photo-grid">
{% assign research_photos = site.static_files | where_exp: "f", "f.path contains 'assets/img/experimental/'" %}
{% for photo in research_photos %}
  {% assign ext = photo.extname | downcase %}
  {% if photo.name == '.gitkeep' or photo.name == '.DS_Store' or ext == '.webp' %}
    {% continue %}
  {% elsif ext == '.mp4' or ext == '.mov' or ext == '.webm' %}
  <video controls muted playsinline preload="metadata"><source src="{{ photo.path | relative_url }}"></video>
  {% else %}
  <img src="{{ photo.path | relative_url }}" alt="" loading="lazy">
  {% endif %}
{% endfor %}
</div>

## Personal

<div class="photo-grid">
{% assign personal_photos = site.static_files | where_exp: "f", "f.path contains 'assets/img/personal/'" %}
{% for photo in personal_photos %}
  {% assign ext = photo.extname | downcase %}
  {% if photo.name == '.gitkeep' or photo.name == '.DS_Store' or ext == '.webp' %}
    {% continue %}
  {% elsif ext == '.mp4' or ext == '.mov' or ext == '.webm' %}
  <video controls muted playsinline preload="metadata"><source src="{{ photo.path | relative_url }}"></video>
  {% else %}
  <img src="{{ photo.path | relative_url }}" alt="" loading="lazy">
  {% endif %}
{% endfor %}
</div>

## Travel

<div class="photo-grid">
{% assign travel_photos = site.static_files | where_exp: "f", "f.path contains 'assets/img/travel/'" %}
{% for photo in travel_photos %}
  {% assign ext = photo.extname | downcase %}
  {% if photo.name == '.gitkeep' or photo.name == '.DS_Store' or ext == '.webp' %}
    {% continue %}
  {% elsif ext == '.mp4' or ext == '.mov' or ext == '.webm' %}
  <video controls muted playsinline preload="metadata"><source src="{{ photo.path | relative_url }}"></video>
  {% else %}
  <img src="{{ photo.path | relative_url }}" alt="" loading="lazy">
  {% endif %}
{% endfor %}
</div>

<style>
.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 1rem;
  margin: 1rem 0 2.5rem;
}
.photo-grid img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: 8px;
  cursor: zoom-in;
}
.photo-grid video {
  width: 100%;
  height: 220px;
  object-fit: contain;
  background: #000;
  border-radius: 8px;
}
</style>
