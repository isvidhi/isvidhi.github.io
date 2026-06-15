<!-- ---
layout: single
title: "Projects"
permalink: /projects/
---

## Industrial Automation Systems
* **Modbus PLC Interface**
    * **Tech:** C++, Qt, Serial Communication
    * [View on GitHub](https://github.com/your-username/repo-name)
    * Designed a high-speed interface for legacy factory hardware.

* **Robotic Arm Controller**
    * **Tech:** C++, ROS2
    * Implemented inverse kinematics for precise trajectory planning. -->

<!-- ---
layout: archive
title: "Projects"
permalink: /projects/
---

{% assign project_list = site.data.projects %}

<div class="feature__wrapper">
  {% for project in project_list %}
    <div class="feature__item">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <p><strong>Stack:</strong> {{ project.stack }}</p>
      <p><a href="{{ project.github }}" class="btn btn--small">View on GitHub</a></p>
    </div>
  {% endfor %}
</div> -->

---
layout: archive
title: "Projects"
permalink: /_pages/projects/
---

{% assign project_list = site.data.projects %}

<div class="feature__wrapper">
  {% for project in project_list %}
    <div class="feature__item">
      <h3>{{ project.title }}</h3>
      
      <!-- GitHub Badges -->
      <p>
        <a href="{{ project.github }}"><img src="https://img.shields.io/github/stars/{{ project.repo_path }}?style=social" alt="Stars"></a>
        <a href="{{ project.github }}"><img src="https://img.shields.io/github/forks/{{ project.repo_path }}?style=social" alt="Forks"></a>
        <img src="https://img.shields.io/github/languages/top/{{ project.repo_path }}?color=blue" alt="Language">
      </p>

      <p>{{ project.description }}</p>
      <p><strong>Stack:</strong> <code>{{ project.stack }}</code></p>
      <p><a href="{{ project.github }}" class="btn btn--small">View Repository</a></p>
    </div>
  {% endfor %}
</div>