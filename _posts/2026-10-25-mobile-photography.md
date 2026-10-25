---
layout: post
title: Mobile Photography
description: Photographs organized by location
date: 2026-10-25 00:00:00 +0800
permalink: /photography/
hidden_from_blog: true
related_posts: false
comments: false
---

<link rel="stylesheet" href="{{ '/assets/css/photography.css' | relative_url }}">

<div class="photo-places">
{% for place in site.data.photography.places %}
  {% assign place_url = place.slug | prepend: '/photography/' | append: '/' %}
  <a class="photo-place" href="{{ place_url | relative_url }}">
    <img src="{{ place.cover | relative_url }}" alt="{{ place.title | escape }}" loading="lazy">
    <span class="photo-place-label">
      <strong>{{ place.title }}</strong>
      <span>{{ place.subtitle }}</span>
    </span>
  </a>
{% endfor %}
</div>

<p class="photo-note">The images above are template examples. My own photographs will be added here.</p>
