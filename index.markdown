---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

Hi! I'm David Wadden. I'm a 5th year PhD student in the [NLP group](https://nlp.washington.edu) at the [University of Washington](https://www.cs.washington.edu), advised by [Hanna Hajishirzi](https://h2lab.cs.washington.edu).

I study Natural Language Processing, with a focus on applications in science and health.


## Publications
<ul>
  {% for paper in site.data.publications.papers%}
    <ul class="list-group">
      <li class="list-group-item">
        <p>
          <b class='text'>{{paper.title}}</b>
          <br>
          <i class='text'>{{ paper.authors }} </i>
          <br>
          <span class='text'>{{paper.conference}} </span>
          <br>
          {% if paper.website %}
          <a class="badge badge-pill badge-warning" href="{{ paper.website}}" target="_blank">Project page</a>
          &nbsp;
          {% endif %}
          {% if paper.dataset %}
          <a class="badge badge-pill badge-danger" href="{{ paper.dataset}}" target="_blank">Dataset</a>
          &nbsp;
          {% endif %}
          {% if paper.pdf %}
          <a class="badge badge-pill badge-primary" href="{{ paper.pdf}}" target="_blank">PDF</a>
          &nbsp;
          {% endif %}
          {% if paper.semanticscholar %}
          <a class="badge badge-pill badge-info" href="{{ paper.semanticscholar}}" target="_blank">Semantic scholar</a>
          &nbsp;
          {% endif %}
          {% if paper.demo %}
          <a class="badge badge-pill badge-secondary" href="{{ paper.demo}}" target="_blank">Demo</a>
          &nbsp;
          {% endif %}
          {% if paper.code %}
          <a class="badge badge-pill badge-success" href="{{ paper.code }}" target="_blank">Source code</a>
          &nbsp;
          {% endif %}
        </p>
      </li>
    </ul>
    {% endfor %}
</ul>
