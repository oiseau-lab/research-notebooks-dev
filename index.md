---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---

Homepage for [oiseau-lab](https://github.com/oiseau-lab)'s GitHub Pages of the [research-notebooks repository](https://github.com/oiseau-lab/research-notebooks).

{% for stakeholder_plot in site.stakeholder_plots %}
  <h2>
    <a href="{{ stakeholder_plot.url }}">
      {{ stakeholder_plot.title }}
    </a>
  </h2>
  <p>{{ stakeholder_plot.content | markdownify }}</p>
{% endfor %}
