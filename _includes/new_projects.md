<h2 id="projects" style="margin: 2px 0px -15px;">Ongoing Projects</h2>

<div class="projects">
<ol class="project-list">

{% for project in site.data.projects.main %}

<li>
<div class="project-container">
    <div class="title-and-img-flexbox">
        <div class="project-title"><strong>{{ project.title }}</strong></div>
        <div class="project-image">
            {% if project.image %} 
             <img src="{{ project.image }}">
            {% endif %}
        </div>
    </div>
    <div class="project-description">{{ project.description }}</div>
    <h3 id="project-literature" style="margin: 2px 0px -15px;">Relevant Literature</h3>
    <div class="project-literature">
        <ul class="literature-list">
        {% for literature in project.literature %}
            <li><a href="{{ literature.link }}" target="_blank">{{ literature.title }}</a></li>
        {% endfor %}
        </ul>
    </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>

