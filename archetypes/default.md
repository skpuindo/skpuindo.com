---
title           : "{{ .File.ContentBaseName | humanize | replaceRE `\s+` " " | title }}"
date            : {{ .Date }}
slug            : "{{ .File.ContentBaseName | urlize }}"  # slug (URL segment) for this post
draft           : true

description     : "Enter the post description (a short SEO-friendly blurb)"
summary         : "Enter a brief summary of the post (used in list previews)"
keywords        : ["SEO keyword 1", "SEO keyword 2", "SEO keyword 3"]
tags            : ["tag a", "tag b", "tag c"]

params:
#  comments:
#    id          : ""  # bsky post id
  neso:
    show_toc    : false  # show the table of contents
#    cover:     # cover image settings (remove this whole block if you have no cover)
#      image    : "<cover image URL>"  # just put the filename if the cover lives in the same bundle as the md
#      caption  : "<cover caption>"    # optional; shown under the cover image
#      alt_text : "<cover alt text>"   # optional; accessibility text
---
