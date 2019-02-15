<p style="padding-left: 2em;">This is our class blog for Code-Paper-Scissors at the School for Poetic Computation in February, 2019.</p>
<ul>
  {% for post in site.posts %}
    {% unless post.hidefromlist %}
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p><b>by {{ post.author }} on {{ post.date | date_to_string }}</b></p>
    <p class="blog-linebreak"><i>{{ post.subtitle }}</i></p>
    {% endunless %}
  {% endfor %}
</ul>
