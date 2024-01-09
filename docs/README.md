# For testing GitHub Pages :)

## Releases

{% for release in site.github.releases %}

{{ release.tag_name }} ({{ release.published_at }})

Changelog: 
{{ release.body }}

Download:
<ul>
{% for asset in release.assets %}
<li><a href="{{ asset.browser_download_url }}">{{ asset.name }}</a></li>
{% endfor %}
</ul>

{% endfor %}
