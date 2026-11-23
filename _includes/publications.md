## Selected Publications

{% for link in site.data.publications.main %}
- **{% if link.pdf %}[{{ link.title }}]({{ link.pdf }}){% else %}{{ link.title }}{% endif %}** — {{ link.authors }}. {{ link.conference }}{% if link.code %} [Code]({{ link.code }}).{% endif %}
{% endfor %}
