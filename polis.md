<h1>Aktuella tillstånd</h1>
Vi försöker hålla listan nedan uppdaterad med aktuella polistillstånd.

<ul>
  {% assign pdfs = site.static_files | where: "extname", ".pdf" %}
  {% assign sorted_pdfs = pdfs | sort: "path" | reverse %}
  {% for file in sorted_pdfs %}
    {% if file.path contains '/assets/permits/' %}
      <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
