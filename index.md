---
layout: default
title: Home
---

<section class="hero" id="home">
    <h1>Professional Cleaning Services</h1>
    <p>Your Trusted Local Cleaning Experts</p>
    <a href="{{ '/contact' | relative_url }}" class="btn">Book Now</a>
</section>

<section class="services" id="services">
    <div class="services-container">
        <h2 class="section-title">Our Services</h2>
        <div class="services-grid">
            {% for service in site.data.services %}
            <div class="service-card">
                <img src="{{ service.icon }}" alt="{{ service.title }}">
                <h3>{{ service.title }}</h3>
                <p>{{ service.description }}</p>
            </div>
            {% endfor %}
        </div>
    </div>
</section>
