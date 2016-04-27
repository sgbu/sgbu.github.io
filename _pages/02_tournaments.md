---
layout: page
title:  "Tournaments"
permalink: /tournaments/
---

  <h2>Tournaments</h2>
  <h4>Hosted by SGBU</h4>
  <div style="overflow-x:auto;">
      <table>
          <tr>
              <th>Date</th>      
              <th>Tournament</th>
          </tr>
          {% for page in site.pages reversed %}
                {% if page.layout == "tournament" %}
                <tr>
                    <td>{{page.date}}</td>
                    <td><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></td>
                </tr>
                {% endif %}
          {% endfor %}

      </table>
  </div>
