---
title: Sotrudniki.net
date: 2020-04-10T15:29:46.534Z
description: Новая система генерации плохих сотрудников
---
<https://mandrillapp.com/track/click/31128206/sotrudniki-net.netlify.com?p=eyJzIjoiY0JUUTBXbEpwVV84NEpoODdVUVAyQzQ2UmJNIiwidiI6MSwicCI6IntcInVcIjozMTEyODIwNixcInZcIjoxLFwidXJsXCI6XCJodHRwOlxcXC9cXFwvc290cnVkbmlraS1uZXQubmV0bGlmeS5jb21cXFwvI2ludml0ZV90b2tlbj13cUREdHJLazBpeGRxTU1ROVgxbGV3XCIsXCJpZFwiOlwiNzg2YzM3YTBiYmM4NGJkMGE3ZGZlMTYzNjJmMGYyOGFcIixcInVybF9pZHNcIjpbXCJlNjBjNGI0NmEzNzJkOTgxNjU3NjQxZTEzNTNhNDQ2MWUzYmY3YTRiXCJdfSJ9>

```editorconfig
backend:
  name: git-gateway
  branch: master

media_folder: static/img
public_folder: /public

collections:
  - name: "blog"
    label: "Blog"
    folder: "content/blog"
    create: true
    slug: "{{year}}-{{month}}-{{day}}-{{slug}}"
    editor:
      preview: false
    fields:
      - { label: "Title", name: "title", widget: "string" }
      - { label: "Publish Date", name: "date", widget: "datetime" }
      - { label: "Description", name: "description", widget: "string" }
      - { label: "Body", name: "body", widget: "markdown" }
```