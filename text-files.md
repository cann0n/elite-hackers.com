---
layout: page
title: Hacking Text Files
hide-nav: true
permalink: /text-files/
summary: Ever since the beginning of hacking in the early 1990's, hackers were writing articles and documenting their findings. Because the internet wasn't invented yet and they didn't have blogs, they would write them using Microsoft Windows Notepad. When I read a hacking text file I find useful, I post it here.
---
{% assign textfiles = site.textfiles %}
<div class="textfiles">
  <table class="pure-table">
    <thead>
      <tr>
        <th>File</th>
        <th>Description</th>
      </tr>
    </thead>
    <tbody>
    {% for textfile in textfiles %}
      <tr>
        <td><a href="/assets/textfiles/{{ textfile.title }}">{{ textfile.title }}</a></td>
        <td>{{ textfile.description }}</td>
      </tr>
    {% endfor %}
    </tbody>
  </table>
</div>
