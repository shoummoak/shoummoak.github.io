<h2 id="publications" style="margin: 2px 0px -15px;">Papers</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li style="list-style-position: inside; padding: 0;">
<div class="pub-row">
  <!-- <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 0px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
    {% endif %}
  </div> -->
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 0px;">
      <div class="title"><a href="{{ link.title_ref }}" target="_blank">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em></div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
<!--       {% if link.notes %} 
      <strong> <i style="color:#000000">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.workshop %} 
      <a href="{{ link.workshop }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Workshop</a>
      {% endif %}
      {% if link.poster %} 
      <a href="{{ link.poster }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Poster</a>
      {% endif %} -->
    </div>
  </div>
  <!--   if workshop -->
  {% if link.workshop_notes %}
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 0px;">
    <div class="periodical"><em>{{ link.workshop_notes }}</em></div>
  </div>
  <div class="links">
      {% if link.workshop %} 
      <a href="{{ link.workshop }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Workshop</a>
      {% endif %}
      {% if link.poster %} 
      <a href="{{ link.poster }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Poster</a>
      {% endif %}
  </div>
  {% endif %}

</div>
</li>
<br>

{% endfor %}

</ol>
</div>
