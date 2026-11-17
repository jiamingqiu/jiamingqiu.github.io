---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======

* Ph.D. in Statistics, Iowa State University, 2022
  * Advisors: [Xiongtao Dai](https://xiongtaodai.com/) and [Zhengyuan Zhu](https://www.stat.iastate.edu/people/zhengyuan-zhu)
* M.S. in Statistics, University of Michigan, Ann Arbor, 2017
* B.S. in Pure and Applied Mathematics, Tsinghua University, 2015

Work Experience
======

* September 2026–present: Postdoctoral Research Associate, University of Southern California, Los Angeles, CA
  * Advisor: [Sze-chuan Suen](https://viterbi.usc.edu/directory/faculty/Suen/Sze-chuan)
* 2022–2026: Postdoctoral Researcher, Fred Hutchinson Cancer Center, Seattle, WA
  * Developed methods for adapting decision rules to distribution shift and optimizing sequential decisions under accuracy, timeliness, and cost constraints, with applications to cancer diagnosis and active surveillance.
  * Advisors: [Yingye Zheng](https://www.fredhutch.org/en/faculty-lab-directory/zheng-yingye.html) and [Yingqi Zhao](https://www.fredhutch.org/en/faculty-lab-directory/zhao-yingqi.html)
* 2020–2022: Graduate Research Assistant, Iowa State University, Ames, IA
  * Project: [Integrating Social and Biophysical Indicators of Nutrient Reduction Progress in Iowa Watershed Projects](https://www.cals.iastate.edu/inrc/projects/2019/integrating-social-and-biophysical-indicators-nutrient-reduction-progress-iowa)
  * Worked on survey data quality control, spatial and temporal imputation methods, and interactive visualization of biophysical and survey data.

Awards
======

* Research Excellence Award, Graduate College, Iowa State University, 2021
* Teaching Excellence Award, Graduate College, Iowa State University, 2020
* George W. Snedecor Award — Most Outstanding Ph.D. Candidate in Statistics, Department of Statistics, Iowa State University, 2019

Publications and Manuscripts
======

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Talks and Presentations
======

{% assign talk_years = site.talks | group_by_exp: "talk", "talk.date | date: '%Y' | default: talk.year | append: ''" | sort: "name" | reverse %}
<ul>{% for year in talk_years %}
  {% for post in year.items reversed %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}
{% endfor %}</ul>

{% comment %}
Teaching Experience
======

{% include teaching-experience.md %}
{% endcomment %}

Service
======

* Reviewer for NeurIPS 2025, *Biometrics*, *Technometrics*, *Statistics and Computing*, and *Biostatistics*
* Committee member, 39th New England Statistics Symposium Student Paper Competition
