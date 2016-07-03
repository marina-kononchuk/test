# test
{% extends 'base.html' %}
{% block section %}

     {% for m in posts %}
        <div class=" col-md-3">
            <a href="{% url 'post' pk=m.id %}" class="thumbnail"
               style="background-image:url({{ m.image.url }}) ">
            </a>
        </div>
    
    {% endfor %}
{% endblock %}
