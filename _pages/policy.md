---
layout: page
title: policy work
permalink: /policy/
nav: true
nav_order: 3
display_categories: [policy]
horizontal: false
---

A growing portfolio of <strong>policy-relevant</strong> research delivered in collaboration with Australian and international stakeholders &mdash; from the [Department of Home Affairs](https://www.homeaffairs.gov.au/) and the [NSW Premier's Department](https://www.nsw.gov.au/departments-and-agencies/premiers-department) to the [Australian Resilient Democracy Network](https://politicsir.cass.anu.edu.au/research/projects/australian-resilient-democracy-network) and [Merseyside Police](https://www.merseyside.police.uk/). The aim of this page is to make the evidence base behind these collaborations available to scholars, policy-makers, and funders in a single place.

<!-- pages/policy.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}
{%- endif -%}
</div>
