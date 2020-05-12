---
layout: default
permalink: /posts/
---

I have separated the write-ups from the blog posts, please navigate accordingly:

[Blog]({% link _pages/blog.md %}): To view the blog posts. | [Write-Ups]({% link _pages/write-ups.md %}): To view the Write-ups.

Or you can search for a specific post across all blog posts and write-ups:

<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="Keyword(s)...">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="../assets/js/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/search.json'
})
</script>

