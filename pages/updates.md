# Updates

{% assign fay-posts = site.posts | where: "tags", "fay" %}
{% assign ed-posts = site.posts | where: "tags", "ed" %}

## From Fay

{% for post in fay-posts %}
  [{{post.title}} - {{post.date | date_to_string}}]({{site.baseurl}}/{{post.url}})
{% endfor %}

## From ED

{% for post in ed-posts %}
  [{{post.title}} - {{post.date | date_to_string}}]({{site.baseurl}}/{{post.url}})
{% endfor %}
