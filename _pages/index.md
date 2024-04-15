---
layout: page
title: Home
id: home
permalink: /
---

# Gm and welcome to my vault


## <strong>My vault</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "title" %}
  {% for note in recent_notes limit: 5 %}
    <li>
      <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
