---
#excerpt: "Exploring graphics, simulation and AI"
header:
    overlay_image: /assets/images/ferro_header_compressed.jpg
    overlay_filter: 0.5
    show_overlay_excerpt: false
    image_description: "2D ferrofluid simulation from my thesis project."
    caption: "Simulation of the Rosensweig instability."
layout: splash
author_profile: false
#classes: wide

#collection: projects
#entries_layout: grid
---

<div class = "frontpageButtonLeftMost">
    <a href="/projects/"> <img class = "frontpageButtonImage" border="0" alt="W3Schools" src="assets/images/projects_thumbnail.jpg" > <div class = "frontpageButtonTextBackdrop"> <span class = "frontpageButtonText"> My Projects </span> </div> </a>
</div>

<div class = "frontpageButton">
    <a href="/about/"> <img class = "frontpageButtonImage" border="0" alt="W3Schools" src="assets/images/mhonke_thumbnail.jpg" > <div class = "frontpageButtonTextBackdrop"> <span class = "frontpageButtonText"> About Me </span> </div> </a>
</div>

<div class = "frontpageButton">
    <a href="https://github.com/mlhonke"> <img class = "frontpageButtonImage" border="0" alt="W3Schools" src="assets/images/github_logo_inverted.svg" > <div class = "frontpageButtonTextBackdrop"> <span class = "frontpageButtonText"> My GitHub </span> </div> </a>
</div>


<div>
<h3>{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}

{% include paginator.html %}
</div>

