---
layout: page
title: Textbook
permalink: /textbook/
---

<p> <b>Textbook</b> [Recommended]:</p>
<p style="margin-left:5%"> Moebs, W., Ling, S. J., & Sanny, J. (2016). <i>University Physics Volume 1.</i> OpenStax.</p>
<p style="margin-left:5%"> Access for free at <a href="https://openstax.org/details/books/university-physics-volume-1" target="_blank"> OpenStax </a></p>

<p><b>Textbook</b> [Recommended, not Required]: </p>
<p style="margin-left:5%"> Knight, R. D. (2022). <i>Physics for Physicists and Engineers, Vol. 1</i> (5th ed.). Pearson. </p>

<!-- <p style="margin-left:5%; margin-top:3%"> <em><u>Mastering Physics</u></em>, an online homework system associated with this textbook, is required. Instructions below. </p> -->

<!-- <div class="thumb_container" style="padding-bottom:1em"> -->
<!--  <a href="https://drive.google.com/file/d/1yyciHs3GIjsXWb-T1bY4H1TKxwnQItyr/view" target="_blank"> -->
<!--    <figure class="thumblink"> -->
<!--      <img class="thumblink-img-portrait" src="{{site.baseurl}}/images/thumbs/MP00.png" alt="Mastering image" > -->
<!--      <figcaption class="thumblink-caption"> Mastering Physics <br> Registration </figcaption> -->
<!--    </figure> -->
<!--  </a> -->
<!-- </div> -->

<hr>

<p style="padding-top:1em"> Closest match between sections in OER textbook (OpenStax) and Pearson textbook </p>

<div>
<table class="oer">
  {% for row in site.data.oer_book %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
</div> 
