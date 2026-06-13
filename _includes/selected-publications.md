<div class="publications selected-publications">
  <ol class="bibliography selected-bibliography">
    {% for link in site.data.conferences.main %}
    {% if link.selected and link.selected_order == 1 %}
    <li class="publication-item selected-publication">
      <div class="pub-row selected-row">
        <div class="selected-media">
          {% assign teaser_image = link.selected_image | default: link.image %}
          {% if link.conference_short %}
          <abbr class="badge selected-venue-tag">{{ link.conference_short }}</abbr>
          {% endif %}
          {% if teaser_image %}
          <img src="{{ teaser_image }}" class="teaser img-fluid z-depth-1" alt="{{ link.teaser_label | default: link.title }}">
          {% endif %}
        </div>
        <div class="publication-content">
          <div class="publication-title-line">
            <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
          </div>
          <div class="author">{{ link.authors }}</div>
          <div class="periodical"><em>{{ link.conference }}</em></div>
          <div class="links">
            {% if link.pdf %}<a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank">PDF</a>{% endif %}
            {% if link.code %}<a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank">Code</a>{% endif %}
            {% if link.page %}<a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank">Page</a>{% endif %}
            {% if link.notes %}<strong><i>{{ link.notes }}</i></strong>{% endif %}
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
          {% if link.journal_short %}
          <abbr class="badge selected-venue-tag">{{ link.journal_short }}</abbr>
          {% endif %}
          {% if teaser_image %}
          <img src="{{ teaser_image }}" class="teaser img-fluid z-depth-1" alt="{{ link.teaser_label | default: link.title }}">
          {% endif %}
        </div>
        <div class="publication-content">
          <div class="publication-title-line">
            <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
          </div>
          <div class="author">{{ link.authors }}</div>
          <div class="periodical"><em>{{ link.journal }}</em></div>
          <div class="links">
            {% if link.pdf %}<a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank">PDF</a>{% endif %}
            {% if link.code %}<a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank">Code</a>{% endif %}
            {% if link.page %}<a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank">Page</a>{% endif %}
            {% if link.notes %}<strong><i>{{ link.notes }}</i></strong>{% endif %}
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
          {% if link.conference_short %}
          <abbr class="badge selected-venue-tag">{{ link.conference_short }}</abbr>
          {% endif %}
          {% if teaser_image %}
          <img src="{{ teaser_image }}" class="teaser img-fluid z-depth-1" alt="{{ link.teaser_label | default: link.title }}">
          {% endif %}
        </div>
        <div class="publication-content">
          <div class="publication-title-line">
            <span class="title">{% if link.pdf %}<a href="{{ link.pdf }}">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}</span>
          </div>
          <div class="author">{{ link.authors }}</div>
          <div class="periodical"><em>{{ link.conference }}</em></div>
          <div class="links">
            {% if link.pdf %}<a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank">PDF</a>{% endif %}
            {% if link.code %}<a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank">Code</a>{% endif %}
            {% if link.page %}<a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank">Page</a>{% endif %}
            {% if link.notes %}<strong><i>{{ link.notes }}</i></strong>{% endif %}
          </div>
        </div>
      </div>
    </li>
    {% endif %}
    {% endfor %}
  </ol>
</div>
