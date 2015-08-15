---
title: RMarkdown Post
layout: post
author: "Civil Servant to the Grand Inquisitor, Jon Chiang"
---



These posts can also be written and saved as a ".Rmd" file. The method is a bit tricky as I have not found a full-proof and simple method, but the following will outline one way.
<!--more-->

In the root file of this website's directory, you'll notice a `_drafts` folder. This folder is intended for all `*.Rmd` files, which I cannot stress enough. In this folder, there will be a file named `r2jekyll.R`. In order to execute this file, we must access its permission by the command `chmod +x`. Yes, those are the letters `chmod`, followed by a **space**, followed by the keys `+x`. 

Assuming you have finished up with your `*.Rmd` file, place it in into the `_drafts` folder rather than the `_posts` folder. Next, access the terminal and run the following command:
	* `./r2jekyll.R rmarkdownpost.Rmd`
This will create 



For example, we create the following plot with the following code:

```r
plot(cars)
```

![plot of chunk car-plot]({{ site.baseurl }}/images/rmarkdown-post-car-plot-1.png) 


