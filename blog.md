<ul>
  {% for post in site.posts %}

    {% unless post.hidefromlist %}
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <small>by {{ post.author }} on {{ post.date | date_to_string }}</small>
    <p>{{ post.subtitle }}</p>
    {% endunless %}
  {% endfor %}
</ul>
