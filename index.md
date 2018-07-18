---
layout: page
title: MarineGEO Data
subtitle: Data Standards and Guidelines
use-site-title: true
---

## Purpose

Collaborative website for people in the MarineGEO network to discover methods, learn data management techniques, and download methods and data entry templates.

## Project Modules

Project modules are packages that contain instructions for deploying experiments, data entry templates and field sheets.

{% assign sorted = site.project-modules | sort: "weight" %}
{% for cat in sorted %}

<div class="col-md-12 col-md-offset-1" style="width: 200px; padding-top: 25px;">
 <a href="{{site.baseurl}}{{cat.url}}">
   <img src="{{ cat.thumbnail }}" class="img-responsive" style="height: 150px; position: relative; left: 50%; top: 50%; margin-left: -75px;">
  <h4 style="text-align:center">{{cat.title}}</h4>
</a>
</div>
{% endfor %}