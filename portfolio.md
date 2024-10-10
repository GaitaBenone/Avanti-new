---
layout: page
title: Portfolio
---

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
  {% for item in site.portfolio %}
    <div class="bg-white rounded-lg shadow-md overflow-hidden">
      {% if item.image %}
        <img src="{{ item.image }}" alt="{{ item.title }}" class="w-full h-48 object-cover">
      {% endif %}
      <div class="p-6">
        <h2 class="text-xl font-bold mb-2">{{ item.title }}</h2>
        <p class="mb-4">{{ item.excerpt | truncate: 100 }}</p>
        <a href="{{ item.url }}" class="text-avanti-teal hover:text-avanti-light-blue font-bold">View Case Study</a>
      </div>
    </div>
  {% endfor %}
</div>