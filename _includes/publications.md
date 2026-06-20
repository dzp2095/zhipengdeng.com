<div class="section-heading publication-heading" id="publications">
  <span class="section-icon" aria-hidden="true"><i class="fas fa-file-alt"></i></span>
  <h2 class="page-title">Publications</h2>
</div>
<p class="publication-note publication-note-top"><sup>*</sup> indicates equal contributions; <i class="fas fa-envelope author-note-icon" title="Corresponding author"></i> indicates corresponding authors.</p>

<div class="publications">
<h3 class="publication-section-title">Selected Publications</h3>
<ol class="bibliography selected-bibliography">
{% for link in site.data.conferences.main %}
{% if link.selected and link.selected_order == 1 %}
<li class="publication-item selected-publication">
  <div class="pub-row selected-row">
    <div class="selected-media">
      {% assign teaser_image = link.selected_image | default: link.image %}
      {% if teaser_image %}
      {% if link.conference_short %}
      <abbr class="badge selected-venue-tag">{{ link.conference_short }}</abbr>
      {% endif %}
      <img src="{{ teaser_image }}" class="teaser img-fluid z-depth-1" alt="{{ link.teaser_label | default: link.title }}" onerror="this.closest('.selected-publication').classList.add('selected-publication-no-image'); this.closest('.selected-media').style.display='none';">
      {% else %}
      {% endif %}
    </div>
    <div class="publication-content">
      <div class="publication-title-line">
        <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
      </div>
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
        <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Page</a>
        {% endif %}
        {% if link.bibtex %}
        <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
        {% endif %}
        {% if link.notes %}
        <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
        {% endif %}
        {% if link.others %}
        {{ link.others }}
        {% endif %}
      </div>
    </div>
  </div>
</li>
{% endif %}
{% endfor %}
{% for link in site.data.journals.main %}
{% if link.selected %}
<li class="publication-item selected-publication">
  <div class="pub-row selected-row">
    <div class="selected-media">
      {% assign teaser_image = link.selected_image | default: link.image %}
      {% if teaser_image %}
      {% if link.journal_short %}
      <abbr class="badge selected-venue-tag">{{ link.journal_short }}</abbr>
      {% endif %}
      <img src="{{ teaser_image }}" class="teaser img-fluid z-depth-1" alt="{{ link.teaser_label | default: link.title }}" onerror="this.closest('.selected-publication').classList.add('selected-publication-no-image'); this.closest('.selected-media').style.display='none';">
      {% else %}
      {% endif %}
    </div>
    <div class="publication-content">
      <div class="publication-title-line">
        <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
      </div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.journal }}</em></div>
      <div class="links">
        {% if link.pdf %}
        <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
        {% endif %}
        {% if link.code %}
        <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
        {% endif %}
        {% if link.page %}
        <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Page</a>
        {% endif %}
        {% if link.bibtex %}
        <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
        {% endif %}
        {% if link.notes %}
        <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
        {% endif %}
        {% if link.others %}
        {{ link.others }}
        {% endif %}
      </div>
    </div>
  </div>
</li>
{% endif %}
{% endfor %}
{% for link in site.data.conferences.main %}
{% if link.selected and link.selected_order != 1 %}
<li class="publication-item selected-publication">
  <div class="pub-row selected-row">
    <div class="selected-media">
      {% assign teaser_image = link.selected_image | default: link.image %}
      {% if teaser_image %}
      {% if link.conference_short %}
      <abbr class="badge selected-venue-tag">{{ link.conference_short }}</abbr>
      {% endif %}
      <img src="{{ teaser_image }}" class="teaser img-fluid z-depth-1" alt="{{ link.teaser_label | default: link.title }}" onerror="this.closest('.selected-publication').classList.add('selected-publication-no-image'); this.closest('.selected-media').style.display='none';">
      {% else %}
      {% endif %}
    </div>
    <div class="publication-content">
      <div class="publication-title-line">
        <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
      </div>
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
        <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Page</a>
        {% endif %}
        {% if link.bibtex %}
        <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
        {% endif %}
        {% if link.notes %}
        <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
        {% endif %}
        {% if link.others %}
        {{ link.others }}
        {% endif %}
      </div>
    </div>
  </div>
</li>
{% endif %}
{% endfor %}
</ol>

<h3 class="publication-section-title">Journal</h3>
<ol class="bibliography text-bibliography">
{% for link in site.data.journals.main %}
{% unless link.selected %}
<li class="publication-item text-publication">
  <div class="publication-content">
    <div class="publication-title-line">
      <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
    </div>
    <div class="author">{{ link.authors }}</div>
    <div class="periodical"><em>{{ link.journal }}</em>{% if link.journal_short %} ({{ link.journal_short }}){% endif %}</div>
    <div class="links">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %}
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %}
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Page</a>
      {% endif %}
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %}
      <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %}
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</li>
{% endunless %}
{% endfor %}
</ol>

<h3 class="publication-section-title">Conference</h3>
<ol class="bibliography text-bibliography">
{% for link in site.data.conferences.main %}
{% unless link.selected %}
<li class="publication-item text-publication">
  <div class="publication-content">
    <div class="publication-title-line">
      <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
    </div>
    <div class="author">{{ link.authors }}</div>
    <div class="periodical"><em>{{ link.conference }}</em>{% if link.conference_short %} ({{ link.conference_short }}){% endif %}</div>
    <div class="links">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %}
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %}
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Page</a>
      {% endif %}
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %}
      <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %}
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</li>
{% endunless %}
{% endfor %}
</ol>

{% assign has_unselected_preprints = false %}
{% for link in site.data.preprints.main %}
{% unless link.selected %}
{% assign has_unselected_preprints = true %}
{% endunless %}
{% endfor %}
{% if has_unselected_preprints %}
<h3 class="publication-section-title">Preprint</h3>
<ol class="bibliography text-bibliography">
{% for link in site.data.preprints.main %}
{% unless link.selected %}
<li class="publication-item text-publication">
  <div class="publication-content">
    <div class="publication-title-line">
      <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
    </div>
    <div class="author">{{ link.authors }}</div>
    <div class="periodical"><em>{{ link.journal }}</em>{% if link.journal_short %} ({{ link.journal_short }}){% endif %}</div>
    <div class="links">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %}
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %}
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Page</a>
      {% endif %}
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %}
      <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %}
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</li>
{% endunless %}
{% endfor %}
</ol>
{% endif %}
</div>
