---
layout: about
title: Home
permalink: /
subtitle: PhD Candidate, Structural Engineering, UC San Diego

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false
  more_info: >
    <p>Structural and Material Engineering Building</p>
    <p>Room 441E</p>
    <p>La Jolla, CA</p>

selected_papers: false # rendered manually mid-page below instead of the fixed end-of-page slot
social: false # includes social icons at the bottom of the page
images:
  slider: true # loads Swiper for the photo carousel below

announcements:
  enabled: false # no _news items yet -- was rendering an empty "No news so far..." placeholder
  scrollable: true
  limit: 5

latest_posts:
  enabled: false # no _posts yet
  scrollable: true
  limit: 3
---

I work on the seismic performance of steel structural systems and the nonstructural components and equipment they support. My approach pairs full-scale physical testing -- shake-table studies, cyclic beam-column subassembly tests, roving-hammer modal surveys -- with finite element modeling in ABAQUS and OpenSees, correlating the two to check analytical predictions against measured behavior. Current work includes prequalifying DuraFuse bolted moment connections for new special moment frame (SMF) construction and retrofit under the AISC cyclic loading protocol, and characterizing the seismic risk to safety-related equipment in nuclear power plants and hospitals. The common thread is closing the gap between how a structure or its contents are assumed to behave in design and how they actually behave under real loading.

## Research

<div class="row row-cols-1 row-cols-md-3 home-preview-cards">
  <div class="col">
    <a href="{{ '/research/#bolted-moment-connections-can-be-prequalified-for-both-new-construction-and-retrofit' | relative_url }}">
      <div class="card h-100 hoverable">
        <div class="card-body">
          <h2 class="card-title">Bolted moment connections</h2>
          <p class="card-text">Can be prequalified for both new construction and retrofit -- 19 specimens across four full-scale subassemblies, tested under the AISC cyclic loading protocol.</p>
        </div>
      </div>
    </a>
  </div>
  <div class="col">
    <a href="{{ '/research/#nonstructural-equipment-often-governs-seismic-risk-independent-of-the-buildings-global-response' | relative_url }}">
      <div class="card h-100 hoverable">
        <div class="card-body">
          <h2 class="card-title">Nonstructural equipment risk</h2>
          <p class="card-text">Often governs independent of the building's global response -- FEM correlation and NLTHA across isolation and damping designs, for nuclear plant and hospital equipment.</p>
        </div>
      </div>
    </a>
  </div>
  <div class="col">
    <a href="{{ '/research/#full-scale-system-identification-catches-as-built-behavior-a-design-stage-model-cant' | relative_url }}">
      <div class="card h-100 hoverable">
        <div class="card-body">
          <h2 class="card-title">Full-scale system identification</h2>
          <p class="card-text">Catches as-built behavior a design-stage model can't -- impact and white-noise testing on a three-story steel testbed building at UCSD's outdoor shake table.</p>
        </div>
      </div>
    </a>
  </div>
</div>

## Outreach

<div class="row row-cols-1 row-cols-md-3 home-preview-cards">
  <div class="col">
    <a href="{{ '/outreach/#shake-table-outreach' | relative_url }}">
      <div class="card h-100 hoverable">
        <div class="card-body">
          <h2 class="card-title">Shake-table outreach</h2>
          <p class="card-text">Running the department's outreach program -- visits, resume workshops, and mentoring, as EERI UCSD chapter president.</p>
        </div>
      </div>
    </a>
  </div>
  <div class="col">
    <a href="{{ '/outreach/#professional-engagement' | relative_url }}">
      <div class="card h-100 hoverable">
        <div class="card-body">
          <h2 class="card-title">CASGC graduate lead</h2>
          <p class="card-text">Leading a summer research program for undergraduates in the California Space Grant Consortium's aerospace program.</p>
        </div>
      </div>
    </a>
  </div>
  <div class="col">
    <a href="{{ '/outreach/#teaching' | relative_url }}">
      <div class="card h-100 hoverable">
        <div class="card-body">
          <h2 class="card-title">Teaching</h2>
          <p class="card-text">TA for four courses across the SE curriculum, from introductory programming to capstone design, 100+ students per offering.</p>
        </div>
      </div>
    </a>
  </div>
</div>

<style>
.home-preview-cards .card-title {
  font-size: 1.15rem;
  line-height: 1.35;
  margin-bottom: 0.5rem;
}
.home-preview-cards .card-text {
  font-size: 0.92rem;
}
</style>

## Latest publication

{% include selected_papers.liquid %}

## Photos

{% include photo_carousel.liquid %}
