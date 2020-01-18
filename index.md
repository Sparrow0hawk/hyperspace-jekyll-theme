---
layout: default
title: Hyperspace by HTML5 UP
---
<!-- Intro -->
<section id="intro" class="wrapper style1 fullscreen fade-up">
	<div class="inner">
		<h1>Hyperspace</h1>
		<p>Just another fine responsive site template designed by <a href="http://html5up.net">HTML5 UP</a><br />
		and released for free under the <a href="http://html5up.net/license">Creative Commons</a>.</p>
		<ul class="actions">
			<li><a href="#one" class="button scrolly">Learn more</a></li>
		</ul>
	</div>
</section>

<!-- One -->
<section id="one" class="wrapper style2 spotlights">
  {% for item in site.data.example.whoWeAre %}
	<section>
		<a href="#" class="image"><img src="images/{{ item.img }}" alt="" data-position="center center" /></a>
		<div class="content">
			<div class="inner">
				<h2>{{ item.name }}</h2>
				<p>{{ item.text }}</p>
				<ul class="actions">
					<li><a href="#" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	{% endfor %}
</section>

<!-- Two -->
<section id="two" class="wrapper style3 fade-up">
	<div class="inner">
		<h2>What we do</h2>
		<p>Phasellus convallis elit id ullamcorper pulvinar. Duis aliquam turpis mauris, eu ultricies erat malesuada quis. Aliquam dapibus, lacus eget hendrerit bibendum, urna est aliquam sem, sit amet imperdiet est velit quis lorem.</p>
		<div class="features">
			{% for item in site.data.example.whatWeDo %}
			<section>
				<span class="icon major fa-{{ item.style }}"></span>
				<h3>{{ item.name }}</h3>
				<p>{{ item.text }}</p>
			</section>
			{% endfor %}
		</div>
		<ul class="actions">
			<li><a href="#" class="button">Learn more</a></li>
		</ul>
	</div>
</section>
