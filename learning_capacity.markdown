---
theme: jekyll-theme-primer
layout: sub-page
title: FFRM
permalink: /learning_capacity/
---
<section class="bg-gray-light py-5 fade-in-center">
  <div class="container-lg p-responsive">

    <div class="text-center fade-in-center">
      <h2 class="alt-h2 mb-4">Learning & Capacity Building</h2>
    </div>

    <div class="mt-4 animate-in">
      <h3 class="alt-h3 mt-3">📘 Course introduction</h3>
      <!-- CMS:section id=learning_capacity_course_introduction -->
      <p class="animate-in">Training materials for the Fossil Fuel Retirement Model (FFRM) introduce how to estimate stranded cost and explore retirement pathways for fossil fuel power plants. A full open course will be linked here when it is published.</p>
      <!-- /CMS:section -->
    </div>

    <div class="mt-4 animate-in">
      <h3 class="alt-h3">🚀 Coming soon</h3>
      <!-- CMS:section id=learning_capacity_coming_soon -->
      <ul class="animate-in">
        <li>Open University course on fossil fuel retirement modelling</li>
        <li>User interface and downloadable teaching materials</li>
        <li>Energy Modelling Community recordings</li>
      </ul>
      <!-- /CMS:section -->
    </div>

    <div class="mt-5 animate-in">
      <h3 class="alt-h3">🌍 Energy Modelling Platforms (EMPs)</h3>
      <!-- CMS:section id=learning_capacity_energy_modelling_platforms_emps -->
      <p class="animate-in">Energy Modelling Platforms train analysts to gather data, run independent studies, and prepare investment proposals. FFRM materials may be included in these events as they become available.</p>
      <!-- /CMS:section -->
      <p class="animate-in">
        <a href="https://climatecompatiblegrowth.com/energy-modelling-platform/" class="btn btn-outline-light">Learn more →</a>
      </p>
    </div>

    <div class="container-lg p-responsive py-4 py-md-6 my-lg-6 animate-in">
      <h3 class="alt-h3 text-center mb-3">🌍 Explore EMP Events</h3>

      <div class="clearfix gutter-spacious">
        {% for event in site.data.learning_events.events %}
        <div class="col-md-4 float-left animate-in mb-4">
          <h3 class="alt-h3 mb-3">{{ event.title }}</h3>
          <p><img src="{{ event.image }}" class="img-fluid" alt="{{ event.alt }}"/></p>
          <p class="text-gray">{{ event.description }}</p>

          {% if event.outputs and event.outputs.size > 0 %}
          <details class="animate-in">
            <summary class="btn btn-sm btn-outline toggle-arrow">Show Outputs</summary>
            <ul class="mt-2">
              {% for output in event.outputs %}
              <li class="animate-in">
                {{ output.flag }} <strong>{{ output.country }}</strong>:
                <a href="{{ output.url }}" target="_blank">{{ output.title }}</a>
              </li>
              {% endfor %}
            </ul>
          </details>
          {% endif %}
        </div>
        {% endfor %}
      </div>

      <div class="clearfix gutter-spacious mt-5">
        <div class="col-md-12 animate-in mb-4">
          <h3 class="alt-h3 mb-3">EMP-Adjacent Events</h3>
          <!-- CMS:section id=learning_capacity_emp_adjacent_events -->
          <p class="text-gray">These additional capacity-building activities have used related energy-modelling methods outside the formal EMP series:</p>
          <!-- /CMS:section -->
          <ul>
            {% for adjacent in site.data.learning_events.adjacent_events %}
            <li class="animate-in">{{ adjacent.flag }}
              <a href="{{ adjacent.url }}" target="_blank">{{ adjacent.title }}</a>
            </li>
            {% endfor %}
          </ul>
        </div>
      </div>
    </div>

  </div>
</section>

<style>
.fade-in-center {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeInUp 1s ease forwards;
}
@keyframes fadeInUp {
  to { opacity: 1; transform: translateY(0); }
}
.animate-in {
  opacity: 0;
  transform: translateY(30px);
  animation: animateIn 0.8s ease-out forwards;
}
@keyframes animateIn {
  from { opacity: 0; transform: translateY(30px); }
  to { opacity: 1; transform: translateY(0); }
}
.col-md-4.float-left {
  display: flex;
  flex-direction: column;
  height: 100%;
}
.col-md-4 img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  object-position: center;
  border-radius: 8px;
}
.toggle-arrow::after {
  content: '↓';
  display: inline-block;
  margin-left: 6px;
}
details[open] .toggle-arrow::after {
  transform: rotate(180deg);
}
</style>
