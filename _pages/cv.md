---
layout: page
permalink: /cv/
title: Resume / CV
nav: true
nav_order: 3
cv_pdf: /assets/pdf/example_pdf.pdf # you can also use external links here
cv_format: rendercv # options: rendercv, jsonresume
description: Two curated versions of my curriculum vitae.
toc:
  sidebar: left
---
I maintain two versions of my CV, curated for the audience:

- **Academic CV** — for postdoctoral positions, faculty roles, and research fellowships. 
- **Industry Résumé** — for data-science/analytics, climate-services & R&D, and environmental-consulting roles. 

{% tabs cv-versions %}

{% tab cv-versions Academic CV %}

<a href="{{ '/assets/pdf/cv_academic.pdf' | relative_url }}" class="btn btn-primary" target="_blank" rel="noopener">Download Academic CV (PDF)</a>

<iframe src="{{ '/assets/pdf/cv_academic.pdf' | relative_url }}" width="100%" height="900px" style="border: 1px solid #ccc; margin-top: 1em;"></iframe>

{% endtab %}

{% tab cv-versions Industry Résumé %}

<a href="{{ '/assets/pdf/cv_industry.pdf' | relative_url }}" class="btn btn-primary" target="_blank" rel="noopener">Download Industry Résumé (PDF)</a>

<iframe src="{{ '/assets/pdf/cv_industry.pdf' | relative_url }}" width="100%" height="900px" style="border: 1px solid #ccc; margin-top: 1em;"></iframe>

{% endtab %}

{% endtabs %}
