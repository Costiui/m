---
title: Acasa
photos:
    
 photos:   
  - image: /photos/berlin-1.jpg
    caption: Berlin 1
  - image: /photos/berlin-2.jpg
    caption: Costiui- Berlin
  - image: /photos/berlin-3.jpg
    caption: Costiui - 2012    
---

<ul class="gallery">
	{% for photo in page.photos %}
		<li style="background-image: url('{{ site.baseurl }}{{ photo.image | resize: "800x800>" }}')"><a title="{{ photo.caption }}" href="{{ site.baseurl }}{{ photo.image }}" data-id="#{{ photo.image | slugify }}" data-caption="{{ photo.caption }}"></a></li>
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

