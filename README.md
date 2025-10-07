# Nochman.github.io
<ul>
{% assign weeks = site.homeworks | sort: "date" %}
{% for hw in weeks %}
  <li>
    <a href="{{ hw.url | relative_url }}">{{ hw.title }}</a>
    <small>({{ hw.date | date: "%B %d, %Y" }})</small>
  </li>
{% endfor %}
</ul>
