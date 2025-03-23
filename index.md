---
layout: default
title: Home
---

<section class="hero">
    <div class="hero-content">
        <h1>Professional Cleaning Services</h1>
        <p>Your Trusted Partner in Home & Office Cleaning</p>
        <a href="/contact" class="cta-button">Book Now</a>
    </div>
</section>

<section id="services" class="services">
    <h2>Our Services</h2>
    <div class="service-grid">
        {% for service in site.data.services %}
        <div class="service-card">
            <div class="service-icon">{% include {{ service.icon }} %}</div>
            <h3>{{ service.title }}</h3>
            <p>{{ service.description }}</p>
        </div>
        {% endfor %}
    </div>
</section>

<section id="about" class="about">
    <div class="about-content">
        <div class="about-text">
            <h2>About Us</h2>
            <p>With over 10 years of experience, CleanPro provides top-quality cleaning services...</p>
        </div>
        <img src="/assets/images/team.jpg" alt="Our Team">
    </div>
</section>
