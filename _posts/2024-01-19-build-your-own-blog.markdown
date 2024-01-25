---
layout: post
title:  "Build your own blog (for free)"
date:   2024-01-19 07:47:29 +0100
author: by Matteo Kosina
description: Build your own blog with jekyll and Github-Pages
tags: Jekyll Github-Pages Blog
---
 ![testimage.png](https://upload.wikimedia.org/wikipedia/commons/4/42/Jekyll_%28software%29_Logo.png)
 
*source: [wikipedia](https://upload.wikimedia.org/wikipedia/commons/4/42/Jekyll_%28software%29_Logo.png)*


Have you ever wanted to start your very own blog for travel, tech or other topics? Now you can and the best part is that it is completely free.

We are going to use Github Pages as our Hosting Service and Jekyll to easily generate static websites based of markdown files.
So let´s get started. 

Firstly we have to install jekyll. Herefore you have to have the following things installed:
- Ruby >= 2.5.0
- RubyGems
- GCC
- Make


Then install jekyll by running:

```` 
gem install jekyll bundler
````
Create a project:

```` 
jekyll new <projectname>
````

Navigate to your project:

```` 
cd <projectname>
````

Start the local development server:
```` 
bundle exec jekyll serve
````

In your _config.yml add your github-username and baseurl:

````
baseurl: "" # the subpath of your site, e.g. /blog
url: "" # the base hostname & protocol for your site, e.g. http://example.com
````

Next up head to Github and create a new public repository and setup Github Pages for it.

To do so, head to your repository´s settings tab > Pages and select the main branch to be the branch you want to use for hosting (or a different one if you prefer to do so).
Next up init a git repository in your project folder and push it to the remote branch you just selected.
After the Github Action of deploying, you can visit your blog via https://yourgithubname.github.io/base-url

That´s it now you can start to play around with your newly created blog. Keep in mind, that changes of files within the /sites directory are overwritten because contents of this directory are generated dynamically.



