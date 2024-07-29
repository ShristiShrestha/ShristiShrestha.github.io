---
layout: dev
title: README
exclude_from_nav: true
---

##  Deploy

`scp -r _site/* chise@webhost.cse.lsu.edu:/home/chise/chise.cse/ -p`

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