---
layout: page
title: The Hague
permalink: /photography/Den_Haag/
nav: false
sitemap: false
images:
  spotlight: true
---

<link rel="stylesheet" href="{{ '/assets/css/photography.css' | relative_url }}">

<p><a href="{{ '/photography/' | relative_url }}">&larr; Mobile Photography</a></p>

{% assign place = site.data.photography.places | where: 'slug', 'new-york' | first %}
<div class="photo-gallery spotlight-group">
{% for photo in place.photos %}
  <figure>
    <a class="spotlight" href="{{ photo.image | relative_url }}" data-description="{{ photo.caption | escape }}">
      <img src="{{ photo.image | relative_url }}" alt="{{ photo.alt | escape }}" loading="lazy">
    </a>
    {% if photo.caption %}<figcaption>{{ photo.caption }}</figcaption>{% endif %}
  </figure>
{% endfor %}
</div>

