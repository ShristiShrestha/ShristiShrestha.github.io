---
layout: dev
title: README
exclude_from_nav: true
---

##  Deploy

- `scp -r _site/* chise@webhost.cse.lsu.edu:/home/chise/chise.cse`
- looks like apache2 is not pointing to the home chise dir, so let's make that sure
  - `cp -r /home/chise/chise.cse/* /var/www/html/chise.cse`

### Setup
- Install Ruby and Jekyll from [here](https://jekyllrb.com/docs/installation/windows/)
- To add dependencies:
  - add `gem <dependency-gem>` in Gemfile
  - run `bundle install`
- Build site
  - run `jekyll build --watch`
- Test site
  - run `jekyll serve`
  - [default] run at localhost:4000


# Notes
- In Jekyll, the files inside the _posts folder need to follow a specific naming convention: YEAR-MONTH-DAY-title.md (e.g., 2024-08-12-my-first-post.md). This convention is required because Jekyll uses the date in the filename to generate permalinks, organize posts by date, and provide features like chronological ordering.