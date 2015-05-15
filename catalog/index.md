---
layout: page
title: Catalog
excerpt: "A catalog of all compositions & arrangements published by Cascadian Music."

---
<table class="table table-condensed all-caps">
  <tr>
    <th>Title</th>
    <th>Artist</th>
    <th>Arranger</th>
    <th>Ensemble</th>
    <th>Price (USD)</th>
  </tr>
{% for post in site.categories.marching %} 
  <article>
    <tr>
      <td><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></td>
      <td><a href="{{ site.url }}{{ post.url }}">{{ post.artist }}</a></td>
      <td><a href="{{ site.url }}{{ post.url }}">{{ post.arranger }}</a></td>
      <td><a href="{{ site.url }}{{ post.url }}">{{ post.categories }} band</a></td>
      <td><a href="{{ site.url }}{{ post.url }}">${{ post.price }}.00</a></td>
    </tr>
  </article>
{% endfor %}
</table>
