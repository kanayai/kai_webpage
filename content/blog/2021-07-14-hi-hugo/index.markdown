---
title: Hi Hugo
author: R package build
date: '2021-07-14'
slug: []
categories: []
tags: []
links:
- icon: door-open
  icon_pack: fas
  name: website
  url: https://allisonhorst.github.io/palmerpenguins/
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/allisonhorst/palmerpenguins/
- icon: newspaper
  icon_pack: far
  name: Blog post
  url: https://education.rstudio.com/blog/2020/07/palmerpenguins-cran/
- icon: magic
  icon_pack: fas
  name: slides
  url: /slides/basicR.html
- icon: magic
  icon_pack: fas
  name: lab
  url: /labs/Lab1.html
---

<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/viz/viz.js"></script>
<link href="{{< blogdown/postref >}}index_files/DiagrammeR-styles/styles.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/grViz-binding/grViz.js"></script>

some text 4

``` r
knitr::include_url("/slides/basicR.html")
```

<iframe src="/slides/basicR.html" width="672" height="400px">
</iframe>

``` r
DiagrammeR::grViz("digraph {
  graph [layout = dot, rankdir = TB]
  
  node [shape = rectangle]        
  rec1 [label = 'Step 1. Wake up']
  rec2 [label = 'Step 2. Write code']
  rec3 [label =  'Step 3. ???']
  rec4 [label = 'Step 4. PROFIT']
  
  # edge definitions with the node IDs
  rec1 -> rec2 -> rec3 -> rec4
  }",
  height = 500)
```

<div id="htmlwidget-1" style="width:672px;height:500px;" class="grViz html-widget"></div>
<script type="application/json" data-for="htmlwidget-1">{"x":{"diagram":"digraph {\n  graph [layout = dot, rankdir = TB]\n  \n  node [shape = rectangle]        \n  rec1 [label = \"Step 1. Wake up\"]\n  rec2 [label = \"Step 2. Write code\"]\n  rec3 [label =  \"Step 3. ???\"]\n  rec4 [label = \"Step 4. PROFIT\"]\n  \n  # edge definitions with the node IDs\n  rec1 -> rec2 -> rec3 -> rec4\n  }","config":{"engine":"dot","options":null}},"evals":[],"jsHooks":[]}</script>
