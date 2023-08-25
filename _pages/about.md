---
layout: about
title: about
permalink: /
subtitle: PhD Candidate, Computer Science, University of Illinois Urbana-Champaign

profile:
  align: left
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular
  address: 

news: true  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons below the profile pic
---


<div style="text-align: justify;">

I am passionate about crafting efficient systems to overcome complex challenges,
striving to unravel intricacies with elegantly simple solutions. 
My problem-solving methodology revolves around harnessing expertise across diverse layers within a system,
 fostering collaboration among components,
 and prioritizing simplicity in design.
This approach has empowered me to
  <a href="/projects/av-safety/"> architect frameworks for safe autonomous driving</a>,
  <a href="/projects/ellipsis/"> enable comprehensive security auditing for real-time systems</a>,
 and <a href="/projects/inc-oc/"> mitigate execution variability stemming from cache coherence mechanisms</a>.
This research is advised by <a href="https://cs.illinois.edu/about/people/faculty/lrs">Prof. Lui Sha</a>, at <a href="https://cps-il.github.io/">Cyber-Physical Systems Integration Lab</a>.

</div>

<br>
<br>


<div class="video-container">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/ONt4fxt-biE?si=b9a-kDg9OUEE6mjA" title="Research Summary" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<br>
<br>



## Projects
---

<!-- pages/projects.md -->
<div class="projects">
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% if project.selected -%}
        {% include projects_horizontal.html %}
      {%- endif -%}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% if project.selected -%}
        {% include projects.html %}
      {%- endif -%}
    {%- endfor %}
  </div>
  {%- endif -%}
</div>

<br>

