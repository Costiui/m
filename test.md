---
layout: photo_set
title: test phot
permalink: /test/
description: "test photo."

photos:
    set: berlin
    size: 5
---

<ul class="gallery">
	{% for photo in page.photos %}
		<li style="background-image: url('{{ site.baseurl }}{{ photo.image | resize: "800x800>" }}')"><a title="{{ photo.caption }}" href="{{ site.baseurl }}{{ photo.image }}" data-id="#maramures#costiui#ronaszek#{{ photo.image | slugify }}" data-caption="{{ photo.caption }}"></a></li>
	{% endfor %}
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
	<li class="spacer"></li>
</ul>

<div class="overlay">
	<a href="#" class="close">&#10005;</a>
	<a class="prev">&lsaquo;</a>
	<a class="next">&rsaquo;</a>
	<p class="caption"></p>
	<img>
</div>
