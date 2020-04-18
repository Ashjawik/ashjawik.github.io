---
# This is the jekyll front-matter
# https://jekyllrb.com/docs/front-matter/

# layout defines the html layout to use
layout: post
# title is used for the html header e.g. SEO
title:  "test post"

# date the article was posted first time
date:   2020-03-28 13:43 +0100

# published: true if post should be rendered by jekyll
published: true

# you can choose to exclude this page from the sitemap
sitemap:
  exclude: false

# enter multiple categories, they will appear on the page
categories: 
  - test

# Jekyll redirect
# https://help.github.com/en/enterprise/2.13/user/articles/redirects-on-github-pages
# https://github.com/jekyll/jekyll-redirect-from
# state the pages where the redirect to this page is coming from
redirect_from:
  - /post/123456789/
  - /post/123456789/my-amazing-post/
---

<!--Add some text here -->
This is awesome it works w/o a year/month/date structure.
