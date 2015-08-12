---
title: RMarkdown Post
layout: post
---



These posts can also be written and saved as a ".Rmd" file. The method is a bit tricky as I have not found a full-proof and simple method, but the following will outline one way.

In the root file of this website's directory, you'll notice a `_drafts` folder. This folder is intended for all `*.Rmd` files, which I cannot stress enough. In this folder, there will be a file named `r2jekyll.R`. In order to execute this file, we must access its permission by the command `chmod +x`. Yes, those are the letters `chmod`, followed by a **space**, followed by the keys `+x`. 

Assuming you have finished up with your `*.Rmd` file, place it in into the `_drafts` folder rather than the `_posts` folder. Next, access the terminal and run the following command:
	* `./r2jekyll.R rmarkdownpost.Rmd`
This will create 



For example, we create the following plot with the following code:

```r
plot(cars)
```

![plot of chunk car-plot](/images/rmarkdown-post-car-plot-1.png) 

There are two things that must be installed for this to work:

 * `knitr` package in R
 * `rinruby` for your respective OS
 	* > sudo gem install rinruby [for MAC users]



#### Cumbersome Details

This process is a bit tedious and more information can be found at this [link](https://sites.google.com/a/ddahl.org/rinruby-users/). Additionally, "...a Jekyll plugin that provides an Rmarkdown "converter" so you can write your posts and pages in Rmarkdown..." is located at this [link](https://github.com/atbradley/jekyll-rmarkdown). Essentially, it says in order to render a ".Rmd" file, we need a plug-in, which is located in the `_plugins` folder. 


