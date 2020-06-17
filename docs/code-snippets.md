---
layout: default
title: Code Snippets
nav_order: 3
---

# Code Snippets
{: .no_toc }

This snippets are to help keep the design of the website consistant.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

----

**PS**: Content insertion areas are display with [ ] around a description of what content should be placed here.

### Accordions

```html
<ul class="accordion" data-accordion data-multi-expand="true" data-allow-all-closed="true">

	<!-- Item [Number] -->
	<li class="accordion-item" data-accordion-item>
		<a href="#" class="accordion-title">[Accordion Item Title]</a>
		<div class="accordion-content" data-tab-content>
			[Content]
		</div>
	</li>

	...

</ul>
```

### Block Box Menu

```html
<section class="block-box">
	<div class="content-tag grid-x text-center">
		<div class="cell small-offset-1 small-10 large-4 large-offset-0">
			<div class="tag-box text-uppercase" tabindex="0" aria-level="2">[Menu Grid Title]</div>
		</div>
	</div>

	<div class="content grid-x grid-margin-y medium-up-2 text-uppercase">
		<div class="cell">
			<a class="title-links" href="[Link]">[Menu Item Text]</a>
		</div>

		...
	</div>
</section>
```

### Boxes

```html
<div id="[Name of Box Section]" class="grid-x grid-margin-x small-up-2 large-up-4" data-equalizer data-equalize-by-row="true">
	<div class="cell">
		<a href="[Link]" class="box-link">
			<div class="callout box text-center" data-equalizer-watch>
				<div class="icon"><i class="fas [FontAwesome Icon]"></i></div>
				<p>
					<strong>[Title]</strong><br />
					<small>[Short Description or Blurb]</small>
				</p>
			</div>
		</a>
  	</div>

  	...
</div>
```

### Content Tag with Border

```html
<div class="content-tag grid-x text-center">
	<div class="cell small-offset-1 small-10 large-4 large-offset-0">
		<div class="tag-box text-uppercase" tabindex="0" aria-level="2">Featured</div>
	</div>
</div>
<div class="content-tag-border"></div>
```

### Image Carousel

```html
<div class="orbit content-carousel" role="region" aria-label="[Name of Image Carousel] Pictures" data-orbit data-swipe>
	<div class="orbit-wrapper">
		<div class="orbit-controls">
			<button class="orbit-previous"><span class="show-for-sr">Previous Slide</span><i class="far fa-chevron-left"></i></button>
			<button class="orbit-next"><span class="show-for-sr">Next Slide</span><i class="far fa-chevron-right"></i></button>
		</div>
		<ul class="orbit-container">
			<li class="is-active orbit-slide">
				<figure class="orbit-figure">
					<img class="orbit-image" src="[Link]" alt="[Alt Text]">
					<figcaption class="orbit-caption">[Caption]</figcaption>
				</figure>
			</li>

			<li class="orbit-slide">
				<figure class="orbit-figure">
					<img class="orbit-image" src="[Link]" alt="[Alt Text]">
					<figcaption class="orbit-caption">[Caption]</figcaption>
				</figure>
			</li>

			<li class="orbit-slide">
				<figure class="orbit-figure">
					<img class="orbit-image" src="[Link]" alt="[Alt Text]">
					<figcaption class="orbit-caption">[Caption]</figcaption>
				</figure>
			</li>

			...
		</ul>
	</div>
	<nav class="orbit-bullets">
		<button class="is-active" data-slide="[0]"><span class="show-for-sr">[First] slide details.</span><span class="show-for-sr">Current Slide</span></button>
		<button data-slide="[1]"><span class="show-for-sr">[Second] slide details.</span></button>
		<button data-slide="[2]"><span class="show-for-sr">[Third] slide details.</span></button>
		...
	</nav>
</div>
```

### Table

```html
<table class="hover">
	<thead class="teal small-text-center large-text-left">
		<tr>
			<th colspan="2">[Table Title]</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td width="[Number/Percentage]">[Data]</td>
			<td width="[Number/Percentage]">[Data]</td>
		</tr>
		...
	</tbody>
</table>
```

### Video Grid

```html
<section id="[Name of Video Grid]" class="top-border">
	<div class="content-tag grid-x">
		<div class="cell small-10 large-4 text-center">
			<div class="tag-box text-uppercase" tabindex="0" aria-level="2">[Video Grid Title]</div>
		</div>
	</div>

	<div class="grid-x grid-padding-x large-up-2">
		<div class="cell">
			<div class="responsive-embed widescreen">
				<iframe src="[Youtube Embed Link]" frameborder="0" allow="encrypted-media" allowfullscreen></iframe>
			</div>
		</div>

		...
	</div>
</section>
```