<h1>Bli stödmedlem</h1>
För att stötta vårt arbete har vi organiserat en formell ideell förening, som används för insamling av medel, hyra av lokaler, etc. Att vara med i stödföreningen är helt frivilligt. Det finns inga medlemsavgifter och i regel bara ett möte per år (årsmötet), där styrelsen väljs. Styrelsen ansvarar sedan för insamling av medel och godkännande av kostnader.

Du kan registrera dig som medlem i stödföreningen <a href="https://forms.gle/osvQvEPCuEPC5E2KA" target="_blank">här</a>.

## Föreningsdokument
<ul>
  {% assign pdfs = site.static_files | where: "extname", ".pdf" %}
  {% assign sorted_pdfs = pdfs | sort: "path" | reverse %}
  {% for file in sorted_pdfs %}
    {% if file.path contains '/assets/association/' %}
      <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
