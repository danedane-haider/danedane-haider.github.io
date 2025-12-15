---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{% bibliography -f {{ site.scholar.bibliography }} %}

</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Remove number prefix from topic headings
  document.querySelectorAll('h2.bibliography').forEach(function(heading) {
    heading.textContent = heading.textContent.replace(/^\d+\.\s*/, '');
  });
});
</script>
