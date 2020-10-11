---
title: Latest News
subtitle: ''
description: This is meta description
menu:
  main:
    name: Blog
    weight: 2

---

      {{ range where .Site.Pages "Section" "blog" }}
        <li><a href="{{ .Permalink }}">{{ .Title }}</a><br /><span class="date">{{ .Date.Format "Mon, Jan 2, 2006" }}</span></li>
        {{ end }}
