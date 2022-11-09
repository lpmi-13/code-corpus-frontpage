---
title: How to use the code corpus API
description: The code corpus API is a restful API with only GET functionality (currently)
layout: layouts/post.njk
---

The code corpus API was born out of an idea to be able to scaffold and support content creators who wanted to use real code to generate their learning activities.

## Current usage

It currently only supports get requests at the following endpoints:

```diff-js
https://api.codecorpus.net/function?language=typescript
```

will return a random function from the typescript function data

```
https://api.codecorpus.net/functions?language=python&page=2
```

will return the second page (10 functions per page) of functions from the python function data.

All functions are returned in json format with the following metadata:

-   language
-   number of lines
-   content
