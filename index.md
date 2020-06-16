---
layout: default
title: Home
nav_order: 1
description: "Taylor Univeristy Documentation Website for Staff & Student Developers"
permalink: /
---

# Taylor University Web Documentation
{: .fs-9 }

This documentation is a collaboration of all developers at Taylor University on how to contribute to the Taylor website within Taylor's web environment. Please update or add any content that is out of date so that documentation stays relevant to the current Taylor web environment.

[Get started](#overview){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/Taylor-University/tu-web-documentation){: .btn .fs-5 .mb-4 .mb-md-0 }

----

## Overview

### Platform/Content Management System

Taylor University using the content management system called [dotCMS](https://dotcms.com/). The version of dotCMS that we are on is v5.2. If you need to see any documentation of the dotCMS platform, you can find it at https://dotcms.com/docs/latest/table-of-content.

### CSS/JS Frameworks

This site is using Zurb's Foundation 6 and has been installed using NodeJS and Gulp. Please see Foundation 6 [Documentation](https://foundation.zurb.com/sites/docs/) for more details on the framework. (**P.S.** Your machine will need have npm installed globally to use the npm commands in the following section.) Please see the [setup page]({{ site.baseurl }}{% link docs/setup.md %}) of how this framework is being used.

### Repository

You will need access to the repository to run compilation of the sass files. Please ask one of the staff developers for access to the repository. The repository contains the following:
- files that have been updated to the dotCMS
- compilation script for sass
- snippets for components used on the website
- templates/layouts
- containers
- widgets

**Please Note**: *All code is worked on outside of dotCMS will need to be uploaded to dotCMS since there is not a good way for dotCMS and Github to integrate at this time.*

----

### Contributing

When contributing to any repository in Taylor's Github organization, please first discuss the change you wish to make via pull request,
email, or any other method with the owners of this repository. The selected manager would merge changes upon acceptance of the changes.

#### How to Contribute

1. Install Jekyll and bundler gems
	```bash
	$ gem install jekyll bundler
	```
2. Clone the repository to your computer
3. Navigate to the repositories folder
	```bash
	$ cd {path}/tu-web-documentation
	```
4. Build the site and run local server
	```bash
	$ bundle exec jekyll serve
	```

If you have trouble getting the serve to run, you may be missing some dependencies. Please see [Github's Jekyll site](https://jekyllrb.com/docs/) for more instructions.

#### Thank you to the contributors of Just the Docs!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>

### Code of Conduct

The Taylor University Web Team is committed to fostering a welcoming community. Our conduct aligns with the Taylor's [Life Together Convenant](https://www.taylor.edu/life-together-covenant) which can be found on Taylor's Website.
