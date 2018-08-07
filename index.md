{% for episode in site.episodes %}

  <h2><a href="{{ episode.url | relative_url }}">Épisode n°{{ episode.numero }}{%if episode.partie %}-{{episode.partie}}{% endif %} : {{ episode.title }}</a></h2>

  <iframe width="560" height="315" src="https://www.youtube.com/embed/{{ episode.id_video }}" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

  <strong><a href="{{ episode.url }}">Lire le récap</a></strong>

  <hr />
{% endfor %}
