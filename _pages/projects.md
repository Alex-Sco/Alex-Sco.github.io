---
layout: page
title: projects
permalink: /projects/
description: Elements build our world. My projects focus on the applications of elemental and isotopic abundance ratios. We are deriving new and more accurate CNO isotopic abundance ratios by revisiting and improving existing methods. We are also testing PDR models across a range of C/N/O elemental abundance ratios, as well as radiative transfer models for the relevant line transitions.
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<div class="projects">

{% comment %}
Original category-based project rendering. This would show every project in
_projects/ whose category appears in display_categories.

{% if site.enable_project_categories and page.display_categories %}
  {% for category in page.display_categories %}
    <a id="{{ category }}" href=".#{{ category }}">
      <h2 class="category">{{ category }}</h2>
    </a>
    {% assign categorized_projects = site.projects | where: "category", category %}
    {% assign sorted_projects = categorized_projects | sort: "importance" %}
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-1 row-cols-md-2">
          {% for project in sorted_projects %}
            {% include projects_horizontal.liquid %}
          {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in sorted_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
    {% endif %}
  {% endfor %}
{% else %}
  {% assign sorted_projects = site.projects | sort: "importance" %}
  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-1 row-cols-md-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.liquid %}
        {% endfor %}
      </div>
    </div>
  {% else %}
    <div class="row row-cols-1 row-cols-md-3">
      {% for project in sorted_projects %}
        {% include projects.liquid %}
      {% endfor %}
    </div>
  {% endif %}
{% endif %}
{% endcomment %}

{% assign visible_project_files = "1_myproject.md,2_myproject.md,3_myproject.md" | split: "," %}
{% assign sorted_projects = site.projects | sort: "importance" %}

{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %}
        {% assign project_file = project.path | split: "/" | last %}
        {% if visible_project_files contains project_file %}
          {% include projects_horizontal.liquid %}
        {% endif %}
      {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% assign project_file = project.path | split: "/" | last %}
      {% if visible_project_files contains project_file %}
        {% include projects.liquid %}
      {% endif %}
    {% endfor %}
  </div>
{% endif %}
</div>
