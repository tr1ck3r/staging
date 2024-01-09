# For testing GitHub Pages :)

## Releases

{% for release in site.github.releases %}

**Version**: {{ release.tag_name }} 

Date: {{ release.published_at }}

Changelog: 
{{ release.body }}

[Download]({{ release.tarball_url }}) 

<ul>
{% for asset in release.assets %}
<li><a href="{{ asset.browser_download_url | relative_url }}">{{ asset.name }}</a></li>
{% endfor %}
</ul>

{% endfor %}
