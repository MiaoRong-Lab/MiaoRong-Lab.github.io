---
layout: page
permalink: /publications/
title: 论文
description: 论文列表按年份倒序展示，可使用关键词筛选。
nav: true
nav_order: 1
---

{% include bib_search.liquid %}

<div class="publications">

{% bibliography --group_by year --group_order descending %}

</div>
