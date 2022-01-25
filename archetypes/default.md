---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
image: "{{ .Date | replace "-" "/" }}/{{ .Name }}/{{ .Name }}.jpg"
#author: "Jeremy Tai Abbett" # use capitalize
draft: true
description: "xxx"
categories: [""]
tags: ["", ""]
---

