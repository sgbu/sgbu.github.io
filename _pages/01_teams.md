---
layout: page
title:  "Teams"
permalink: /teams/
---

# National Teams

<table>
    <tr><th>Date</th><th>Tournament</th><th>Division</th><th>Result</th><th>Spirit</th></tr>
    {% for page in site.pages reversed %}
          {% if page.layout == "sg_team" %}
          <tr>
              <td>{{ page.date | date: "%Y" }}</td>
              <td><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></td>
              <td>{{page.division}}</td>
              <td>{{page.place}}</td>
              <td>{{page.spirit}}</td>
          </tr>
          {% endif %}
    {% endfor %}
</table>

# Club Teams

<table>
    <tr><th>Date</th><th>Tournament</th><th>Team</th><th>Result</th></tr>
    {% for page in site.pages reversed %}
          {% if page.layout == "team" %}
          <tr>
              <td>{{ page.date | date: "%Y" }}</td>
              <td><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></td>
              <td>{{page.team}}</td>
              <td>{{page.place}}</td>
          </tr>
          {% endif %}
    {% endfor %}
</table>

## Appendix Ultimate

* **Established:** 2012
* **Division:** Mixed
* **Goal:** Grow Beach Ultimate and its players.
* **Ethos:** [Appendix Ethos](https://docs.google.com/document/d/1JjIVbyXe3vasj9OZ3f3Z13G9qWLu3WuIbIyMODaf8Qw/edit?usp=sharing)
* **Link:** [Ultimate Central](http://ultimatecentral.com/t/appendix-ultimate)

## Skettos

* **Established:** 2015
* **Division:** Mixed
* **Goal:** Win [Chennai Heat 2015](https://www.facebook.com/events/462232350614494/)
