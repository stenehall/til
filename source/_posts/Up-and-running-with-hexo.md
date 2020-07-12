---
title: Up and running with hexo
date: 2020-04-20 15:26:39
tags:
---

```bash
  $ npm install -g hexo
  $ hexo init my-new-blog
  $ cd my-new-blog
  $ npm run server
```

To get Github deploys. Given the documentation you're not supposed to need to provide branch and message but for some reason I had to.

```yaml
deploy:
  type: git
  repo: https://github.com/stenehall/til
  branch: gh-pages
  message: "Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }}"
```
