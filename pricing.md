---
layout: page
title: Pricing
---

{% for plan in site.data.pricing %}
<div class="bg-white rounded-lg shadow-md p-6 mb-8">
  <h2 class="text-2xl font-bold mb-4">{{ plan.name }}</h2>
  <p class="text-3xl font-bold text-avanti-teal mb-4">{{ plan.price }}</p>
  <p class="mb-4">{{ plan.description }}</p>
  <ul class="mb-6">
    {% for feature in plan.features %}
    <li class="flex items-center mb-2">
      <svg class="w-4 h-4 mr-2 text-green-500" fill="currentColor" viewBox="0 0 20 20">
        <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"/>
      </svg>
      {{ feature }}
    </li>
    {% endfor %}
  </ul>
  <a href="#" class="bg-avanti-teal hover:bg-avanti-light-blue text-white font-bold py-2 px-4 rounded-full transition duration-300">Choose Plan</a>
</div>
{% endfor %}