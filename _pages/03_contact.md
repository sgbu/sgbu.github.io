---
layout: page
title:  "Contacts"
permalink: /contact/
locations: 1.247600,103.8240000
zoom: 16
---

{% if page.locations %}
<img src="http://maps.googleapis.com/maps/api/staticmap?{% for location in page.locations %}{% if forloop.first %}center={{location}}&markers=color:blue%7C{{location}}{% else %}&markers=color:blue%7C{{location}}{% endif %}{% endfor %}&zoom={% if page.zoom %}{{page.zoom}}{% else %}13{% endif %}&size=300x200&scale=2&sensor=false&visual_refresh=true" alt="">
{% endif %}
