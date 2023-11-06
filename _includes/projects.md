<h2 id="projects" style="margin: 2px 0px -15px;">Ongoing Projects</h2>

<div class="projects">
<ol class="project-list">

{% for project in site.data.projects.main %}

<li>
<div class="project-row">
    <div class="project-image" style="position: relative;padding-right: 15px;padding-left: 15px;">
        {% if project.image %} 
         <img src="{{ project.image }}" style="width=100;height=40%">
        {% endif %}
    </div>
    <div class="project-details" style="position: relative padding-right: 15px;padding-left: 20px;">
        <div class="project-title"><strong>{{ project.title }}</strong></div>
        <div class="project-description">{{ project.description }}</div>
        <div class="project-literature">
            <ul class="literature-list">
                {% for literature in project.literature %}
                <li><a href="{{ literature.link }}" target="_blank">{{ literature.title }}</a></li>
                {% endfor %}
            </ul>
        </div>
    </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>

