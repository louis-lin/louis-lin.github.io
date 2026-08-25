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

{% include research_cycler.liquid %}

## Outreach

{% include outreach_cycler.liquid %}

## Latest publication

{% include selected_papers.liquid %}

## Photos

{% include photo_carousel.liquid %}

<script>
document.addEventListener("DOMContentLoaded", () => {
  const bio = document.querySelector('article > .clearfix > p:first-of-type');
  const profile = document.querySelector('article > .profile');
  if (!bio || !profile) return;
  const matchHeight = () => { profile.style.height = bio.offsetHeight + 'px'; };
  matchHeight();
  window.addEventListener('resize', matchHeight);
});
</script>

<style>
article > .profile {
  display: flex;
  flex-direction: column;
  overflow: hidden;
}
article > .profile figure {
  flex: 1;
  min-height: 0;
  margin: 0;
}
article > .profile figure picture,
article > .profile figure img {
  height: 100%;
  width: 100%;
  object-fit: cover;
  object-position: center 15%; /* bias crop toward the top so it doesn't cut into the head */
}
article > .profile .more-info {
  flex-shrink: 0;
}

.home-cycler {
  margin: 1rem 0 2.5rem;
  height: 480px;
  border-radius: 8px;
  --swiper-navigation-size: 24px;
}
.cycler-empty {
  margin: 1rem 0;
  padding: 2rem;
  text-align: center;
  border: 1px dashed;
  border-radius: 8px;
  opacity: 0.6;
}
.home-cycler img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 8px;
}
.home-cycler swiper-slide {
  position: relative;
}
.cycler-caption {
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  margin: 0;
  padding: 0.75rem 1rem;
  background: rgba(0, 0, 0, 0.55);
  color: #fff;
  font-size: 0.95rem;
}
.cycler-link {
  margin-top: -1.5rem;
  text-align: right;
}
</style>
