---
layout: default
title: Home
---
Welcome to my mathematical blog. I use this space for notes,
proofs, examples, and explanations.
## Recent posts
{% if site.posts.size > 0 %}
{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
*{{ post.date | date: "%d %B %Y" }}*
{{ post.excerpt }}
[Read the post]({{ post.url | relative_url }})
{% endfor %}
{% else %}
No posts yet.
{% endif %}