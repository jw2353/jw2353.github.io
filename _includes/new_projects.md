<h2 id="projects" style="margin: 2px 0px -15px;">Ongoing Projects</h2>

<div class="projects">
<ol class="project-list">

{% for project in site.data.projects.main %}

<li>
    <ul class="title-and-img-container">
        <li class="project-title"><strong>{{ project.title }}</strong></li>
        <li class="project-image">
            {% if project.image %} 
             <img src="{{ project.image }}">
            {% endif %}
        </li>
    </ul>
    <div class="project-description">{{ project.description }}</div>
    <h3 id="project-literature" style="margin: 2px 0px -15px;">Relevant Literature</h3>
    <div class="project-literature">
        <ul class="literature-list">
        {% for literature in project.literature %}
            <li><a href="{{ literature.link }}" target="_blank">{{ literature.title }}</a></li>
        {% endfor %}
        </ul>
    </div>
</li>

<br>

{% endfor %}

</ol>
</div>

