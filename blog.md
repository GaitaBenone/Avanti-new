---
layout: page
title: Blog
---

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
  {% for post in site.posts %}
    <div class="bg-white rounded-lg shadow-md overflow-hidden">
      {% if post.image %}
        <img src="{{ post.image }}" alt="{{ post.title }}" class="w-full h-48 object-cover">
      {% endif %}
      <div class="p-6">
        <h2 class="text-xl font-bold mb-2">{{ post.title }}</h2>
        <p class="text-gray-600 mb-4">{{ post.date | date: "%B %d, %Y" }}</p>
        <p class="mb-4">{{ post.excerpt | truncate: 100 }}</p>
        <a href="{{ post.url }}" class="text-avanti-teal hover:text-avanti-light-blue font-bold">Read More</a>
      </div>
    </div>
  {% endfor %}
</div>