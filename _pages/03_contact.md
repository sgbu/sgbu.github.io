---
layout: page
title:  "Contacts"
permalink: /contact/
locations: 1.247600,103.8240000
zoom: 16
---
{% if page.locations %}
<img style="float: right;" src="http://maps.googleapis.com/maps/api/staticmap?{% for location in page.locations %}{% if forloop.first %}center={{location}}&markers=color:blue%7C{{location}}{% else %}&markers=color:blue%7C{{location}}{% endif %}{% endfor %}&zoom={% if page.zoom %}{{page.zoom}}{% else %}13{% endif %}&size=200x200&scale=2&sensor=false&visual_refresh=true" alt="">
{% endif %}

Where
--
110 Tanjong Beach Walk, Sentosa
Far end of Palawan Beach, former Dolphin Lagoon
098943 Singapore

When
--
- Regular pick-up _almost_ every saturday from 4.30pm onwards:
- Appendix beginner training _almost_ every saturday from 3.30pm onwards
- Appendix regular training _almost_ every saturday from 2.30pm onwards

For more exact details, check our <a href="https://telegram.me/{{ site.telegram }}"><i class="svg-icon telegram"></i>Telegram</a> channel or our <a href="https://www.facebook.com/groups/{{ site.facebook }}"><i class="svg-icon facebook"></i>Facebook</a> page
