---
layout: post
title: Setup your Jekyll blog and host it at GitHub Pages
---

In this post we will see the steps needed to create a Jekyll blog based on [Poole](http://getpoole.com/) and, first preview it locally and later host it at [Github Pages](https://pages.github.com/). 

To preview our blog locally without pushing changes to GitHub we have to follow these steps:

1. Install jekyll. 

	```
	sudo gem install jekyll
	```
2. Clone Poole repository

   ```
   git clone https://github.com/poole/poole.git
   ```
3. Enter the created poole folder.

   ```
   cd poole
   ```
4. Start jekyll
   
   ```
   jekyll serve --watch
   ```
5. Our blog should be accessible at [localhost:4000](http://localhost:4000)

Once we have Jekyll running locally, let's host our blog at GitHub pages. 

1. Create GitHub account if you don´t have already one. Go to [GitHub](www.github.com) to create it.

2. Create a repository with the name $USERNAME$.github.io

3. In our poole/ folder execute 

	```
	git push --mirror https://github.com/$USERNAME$/$USERNAME$.github.io
	```
	
4. In a few minutes check $USERNAME$.github.io page and we will see our blog :)

## Sources
Here are some links that helped me configure my blog:

* [How I Created a Beautiful and Minimal Blog Using Jekyll, Github Pages, and poole](http://joshualande.com/jekyll-github-pages-poole/)
* [How to host your blog at GitHub using Jekyll and Poole](http://byverdu.github.io/how-to-host-your-blog-at-github-using-jekyll-and-poole/)
* [Jekyll](http://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/)

