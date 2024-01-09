# For testing GitHub Pages :)

## Releases

{% for release in site.github.releases %}

**Version**: {{ release.tag_name }} 

Date: {{ release.published_at }}

Changelog: 

{{ release.body }}

[Download]({{ release.tarball_url }}) 

{% endfor %}
