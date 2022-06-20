---
date: {{ .Date }}
draft: true
title: "{{ .Name | humanize | title }}"
subtitle: ""
location: ""
address: ""
city: ""
country: "it"
{{- $d := .Date | time.AsTime -}}
{{- $d = $d.AddDate 0 0 1 }}
eventDateTime: {{ $d.Format "2006-01-02T15:04:05Z07:00" }}
eventLink: ''
outputs:
- HTML
- Calendar
---