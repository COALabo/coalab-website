---
layout: default
title: Projects
permalink: /projects/
---

# Research Projects

Our lab conducts research across multiple projects that span computational linguistics, bilingualism, and cognitive science. Below are some of our current and recent projects.

## Active Projects

<div class="row">
{% assign active_projects = site.projects | where: "status", "active" %}
{% for project in active_projects %}
    <div class="col-md-6 mb-4">
        <div class="card h-100">
            <div class="card-body">
                <h3 class="card-title h4"><a href="{{ project.url | relative_url }}" class="text-decoration-none">{{ project.title }}</a></h3>
                <p class="card-text">{{ project.excerpt }}</p>
                <div class="mt-3">
                    {% for tag in project.tags %}
                    <span class="badge bg-light text-dark border me-1">{{ tag }}</span>
                    {% endfor %}
                </div>
            </div>
            <div class="card-footer bg-transparent border-top-0">
                <a href="{{ project.url | relative_url }}" class="btn btn-primary btn-sm">Read More</a>
            </div>
        </div>
    </div>
{% endfor %}
</div>

## Completed Projects

<div class="row">
{% assign completed_projects = site.projects | where: "status", "completed" %}
{% for project in completed_projects %}
    <div class="col-md-6 mb-4">
        <div class="card h-100 bg-light">
            <div class="card-body">
                <h3 class="card-title h5 text-muted">{{ project.title }}</h3>
                <p class="card-text small">{{ project.excerpt }}</p>
            </div>
            <div class="card-footer bg-transparent border-top-0">
                <a href="{{ project.url | relative_url }}" class="btn btn-outline-secondary btn-sm">View Archive</a>
            </div>
        </div>
    </div>
{% endfor %}
</div>

## Project Resources

### Data & Code
We believe in open science. Where possible, we make our data and code publicly available:

- [GitHub Organization](https://github.com/coalab)
- [Open Science Framework](https://osf.io/coalab/)
- [Project Datasets](https://dataverse.harvard.edu/dataverse/coalab)

### Collaboration Opportunities
We welcome collaborations on these and related projects. If you're interested in collaborating, please:
1. Review our [Research](/research) page to understand our focus areas
2. Contact the relevant project lead directly
3. Or use our [general contact form](/contact)

### Student Involvement
Many of our projects offer opportunities for student involvement at various levels:
- **Undergraduate students:** Research assistant positions, summer internships
- **Master's students:** Thesis projects, research practicums
- **PhD students:** Dissertation research, long-term project involvement

For information about joining our lab as a student, see our [Contact & Join page](/contact).
