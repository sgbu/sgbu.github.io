---
layout: page
title:  "Teams"
permalink: /team/
---

  <h2>Appendix Ultimate</h2>
  <table>
      <tr>
          <th>Date</th>      
          <th>Tournament</th>
          <th>Place</th>
      </tr>
      {% for page in site.pages reversed %}
            {% if page.layout == "team" %}
            <tr>
                <td>{{page.date}}</td>
                <td><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></td>
                <td>{{page.place}}</td>
            </tr>
            {% endif %}
      {% endfor %}

  </table>
