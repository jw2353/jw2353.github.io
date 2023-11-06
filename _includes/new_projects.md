<h2 id="projects" style="margin: 2px 0px -15px;">Ongoing Projects</h2>

<div class="project-container">
  {% for project in site.data.projects.main %}
  <div class="project">
    <div class="project-text">
      <div class="project-title">{{ project.title }}</div>
      <div class="project-description">{{ project.description }}</div>
      <div class="project-literature">
        <h3>Relevant Literature</h3>
        <ul>
          {% for literature in project.literature %}
          <li><a href="{{ literature.link }}">{{ literature.title }}</a></li>
          {% endfor %}
        </ul>
      </div>
    </div>
    <div class="project-image">
      <img src="{{ project.image }}" alt="Image for {{ project.title }}">
    </div>
  </div>
  {% endfor %}
</div>
