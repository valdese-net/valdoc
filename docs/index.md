---
title: Valdoc Home
---
# Valdoc

<table>
  {% for row in site.data.burkefd %}
    {% if forloop.first %}
      <thead>
        <tr>
          {% for pair in row %}
            <th>{{ pair[0] }}</th>
          {% endfor %}
        </tr>
      </thead>
    {% else %}
      <tr>
        {% for pair in row %}
          <td>{{ pair[1] }}</td>
        {% endfor %}
      </tr>
    {% endif %}
  {% endfor %}
</table>