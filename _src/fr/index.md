---
layout: fr/default.liquid
title: faith.rodeo
---
<div class="head">
    <h1 class="index-header">{{ page.title }}</h1>
    <p class="centre large-paragraph">
        Nous sommes un groupe des gens qui écrivent parfois.
    </p>
</div>

{% for post in collections.posts.pages %}

## [{{ post.title }}]({{ post.permalink }}) - par {{ post.data.author }}
<p class="date">{{ post.data.date }}</p>
{{ post.excerpt}}
<hr>

{% endfor %}

