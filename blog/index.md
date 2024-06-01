{% for post in site.posts limit:5 %}  

<div class="card">
      <div class="card-body">
        <h5 class="card-title"><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h5>
        {% if post.excerpt %}
                  <p class="card-text">{{ post.excerpt }}</p>
        {% endif %}
        <a href="{{ BASE_PATH }}{{ post.url }}" class="btn btn-primary">Read more</a>
      </div>
    </div>
  <li></li>  
{% endfor %}  