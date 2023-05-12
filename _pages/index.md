---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  👋 hi there, I'm Chad. This is my collection of ideas. AKA a digital garden.
</p>
I'm just starting this garden as of May 12, 2023 so it's pretty sparse around here. I'll be adding to it. Thanks for visiting. 

I'm interested in [[acting]], [[analog photography]], [[Buddhism]], [[Absurdism]] as a philosphy, [[animation]], [[sketchnotes]] and [[graphic facilitation]], [[futures thinking]], and [[sketch comedy]].

### Want to make your own garden?

* This digital garden template is free, open-source, and [available on GitHub here](https://github.com/maximevaillancourt/digital-garden-jekyll-template).
* The easiest way to get started is to read this [step-by-step guide explaining how to set this up from scratch](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll).

### Recently updated notes

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
