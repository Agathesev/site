---
layout: default
wide: true
---
<div class="post">

  <article class="post-content">
    <span class="pre-header">{{ page.section }}</span>
    <h1 class="post-title">{{ page.title }}</h1>
    {% if page.authors %}
    <div class="author">Ecrit par
      <ul>
      {% for author in page.authors %}
        <li>{{ author }}</li>
      {% endfor %}
      </ul>
    </div>
    {% endif %}
    {{ content }}
  </article>

</div>

{% include page-tools.html %}
