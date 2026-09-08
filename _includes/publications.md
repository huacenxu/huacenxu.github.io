## Selected Publications

{% for link in site.data.publications.main %}
- **[{{ link.title }}]({{ link.pdf }})** — {{ link.authors }}. {{ link.conference }}{% if link.code %} [Code]({{ link.code }}).{% endif %}
{% endfor %}
