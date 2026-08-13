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

{% include photo_grid.liquid dir="assets/img/experimental/" %}

## Personal

{% include photo_grid.liquid dir="assets/img/personal/" %}

## Travel

{% include photo_grid.liquid dir="assets/img/travel/" %}

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
