---
layout: page
title: Parkrun
permalink: /parkrun/
---

I got involved in doing my local Hartlepool Parkrun and try to run it on a regular basis. This is a list of my results.

### Results

<table>
    <thead>
        <td>Run Number</td>
        <td>Date</td>
        <td>Time</td>
        <td>Position</td>
        <td>PB</td>
    </thead>
    <tbody>
        {% for run in site.runs %}
        <tr>
            <td>{{ run.number }}</td>
            <td>{{ run.date |  date: "%d/%m/%Y" }}</td>
            <td>{{ run.time }}</td>
            <td>{{ run.position }}</td>
            <td>{{ run.pb }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

{% for run in site.runs %}
  <h2>{{ run.position }}</h2>
  <p>{{ run.time }}</p>
  <p>{{ run.pb }}</p>
{% endfor %}