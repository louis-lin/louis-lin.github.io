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

Drop images into `assets/img/experimental/` -- they show up here automatically, no template edits needed.

<div class="photo-grid">
{% assign research_photos = site.static_files | where_exp: "f", "f.path contains 'assets/img/experimental/'" %}
{% for photo in research_photos %}
  {% unless photo.name == '.gitkeep' %}
  <img src="{{ photo.path | relative_url }}" alt="" loading="lazy">
  {% endunless %}
{% endfor %}
</div>

## Personal

Drop images into `assets/img/personal/`.

<div class="photo-grid">
{% assign personal_photos = site.static_files | where_exp: "f", "f.path contains 'assets/img/personal/'" %}
{% for photo in personal_photos %}
  {% unless photo.name == '.gitkeep' %}
  <img src="{{ photo.path | relative_url }}" alt="" loading="lazy">
  {% endunless %}
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
</style>
