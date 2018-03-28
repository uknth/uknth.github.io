---
layout: default
---
<div>
<ul class="link">
{% for post in site.posts %}	
<li class="link">
    <a class="link" style="float:left; font-size:1.2em" href="{{ post.url }}">- {{ post.title }}</a>
    <small style="float:right; margin-top:8px;"><strong>{{ post.date | date: "%B %e, %Y" }}</strong> . {{ post.category }}</small>
</li>
{% endfor %}	
</ul>
</div>
