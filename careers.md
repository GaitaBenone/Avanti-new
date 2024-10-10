---
layout: page
title: Careers at AvantiCart
---

<p class="mb-8">Join our team and help shape the future of ecommerce. At AvantiCart, we're always looking for talented individuals who are passionate about creating innovative solutions for online businesses.</p>

<h2 class="text-2xl font-bold mb-4">Open Positions</h2>

{% for position in site.data.careers %}
<div class="bg-white rounded-lg shadow-md p-6 mb-8">
  <h3 class="text-xl font-bold mb-2">{{ position.title }}</h3>
  <p class="mb-4">{{ position.description }}</p>
  <a href="#" class="text-avanti-teal hover:text-avanti-light-blue font-bold">Learn More & Apply</a>
</div>
{% endfor %}

<p class="mt-8">Don't see a position that fits your skills? We're always interested in hearing from talented individuals. Send your resume to <a href="mailto:careers@avanticart.com" class="text-avanti-teal hover:text-avanti-light-blue">careers@avanticart.com</a>.</p>