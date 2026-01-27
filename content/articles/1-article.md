+++
date = '2025-12-03T00:24:09-05:00'
draft = true
title = 'First Article'
summary = 'An experimental page created for testing Go Hugo'
description = 'Always try before you buy.  Thats what dad always said.'
artists = ["Martin"]
+++

This page is created as a new archetype called `article`, but I did not create an archetype definition yet.  It's really just a new folder under content.

{{ $pages := where site.RegularPages "Type" "posts" }}
{{ $paginator := .Paginate $pages.ByTitle 7 }}

{{ range $paginator.Pages }}
  <h2><a href="{{ .RelPermalink }}">{{ .LinkTitle }}</a></h2>
{{ end }}

{{ partial "pagination.html" . }}