---
layout: page
permalink: /cv/
title: Résumé / CV
nav: true
nav_order: 3
cv_pdf: /assets/pdf/example_pdf.pdf # you can also use external links here
cv_format: rendercv # options: rendercv, jsonresume
description: Please find the suitable one as per requirement. 
toc:
  sidebar: left
---
{% include no_search_hint.liquid %}
 
I maintain two versions of my Résumé/CV, curated as:

- **Academic CV** — regarding postdoctoral positions, faculty roles, and research fellowships. 
- **Industry Résumé** — regarding data-science and analytics, climate-services and related R&D, and environmental-consulting roles. 

<div class="cv-tabs" role="tablist">
  <button class="cv-tab-btn active" onclick="showCvTab(event,'academic')" role="tab">Academic CV</button>
  <button class="cv-tab-btn" onclick="showCvTab(event,'industry')" role="tab">Industry Résumé</button>
</div>

<div id="cv-academic" class="cv-tab-pane active" role="tabpanel">
  <p><a href="{{ '/assets/pdf/cv_academic.pdf' | relative_url }}" class="btn btn-primary" target="_blank" rel="noopener">Download Academic CV (PDF)</a></p>
  <iframe src="{{ '/assets/pdf/cv_academic.pdf' | relative_url }}" width="100%" height="900px" style="border:1px solid #ccc;"></iframe>
</div>

<div id="cv-industry" class="cv-tab-pane" role="tabpanel">
  <p><a href="{{ '/assets/pdf/cv_industry.pdf' | relative_url }}" class="btn btn-primary" target="_blank" rel="noopener">Download Industry Résumé (PDF)</a></p>
  <iframe src="{{ '/assets/pdf/cv_industry.pdf' | relative_url }}" width="100%" height="900px" style="border:1px solid #ccc;"></iframe>
</div>

<style>
.cv-tabs { display:flex; gap:.5rem; margin:1rem 0; border-bottom:2px solid var(--global-divider-color,#ccc); }
.cv-tab-btn { padding:.5rem 1rem; background:transparent; border:none; cursor:pointer;
              font-weight:500; font-size:1rem; color:inherit;
              border-bottom:3px solid transparent; margin-bottom:-2px; }
.cv-tab-btn:hover { opacity:.75; }
.cv-tab-btn.active { border-bottom-color: var(--global-theme-color, currentColor); }
.cv-tab-pane { display:none; }
.cv-tab-pane.active { display:block; }
</style>

<script>
function showCvTab(evt, name){
  document.querySelectorAll('.cv-tab-pane').forEach(el=>el.classList.remove('active'));
  document.querySelectorAll('.cv-tab-btn').forEach(el=>el.classList.remove('active'));
  document.getElementById('cv-'+name).classList.add('active');
  evt.currentTarget.classList.add('active');
}
</script>
