---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: splash
excerpt: "Welcome to my little, tiny bit of place on the internet!"
header:
  overlay_image: /assets/images/header.jpg 
  #overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**Pinterest**](https://www.pinterest.es/pin/546765211014373118/)"
  #actions:
  #  - label: "More Info"
  #    url: "https://unsplash.com"
permalink: /
---
<h2> All posts </h2>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

{% for tag in site.tags %}
  <h2>{{ tag[0] | capitalize}}</h2>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}