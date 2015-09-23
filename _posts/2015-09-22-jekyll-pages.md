---
layout:     post
title:      Jekyll and Github Pages
date:       2015-09-22 11:00:00
summary:    Test
categories: jekyll
thumbnail: cogs
tags:
 - jekyll
 - github
---

###Getting Started with Jekyll and Github Pages###
---
This is a simple quick-start guide to getting started with [Jekyll](https://jekyllrb.com/) and [Github Pages](https://pages.github.com/) to create a personal themed webpage. This guide will be specific to Ubuntu (with similar steps for other linux distros). 

####Prerequisites####
---

* [Git](https://git-scm.com/)  
```~$ sudo apt-get install git```

* [Ruby](https://www.ruby-lang.org/en/)  
```~$ sudo apt-get install ruby```  
```~$ sudo apt-get install ruby-dev```

* [node.js](https://nodejs.org/en/)  
```~$ sudo apt-get install nodejs```

* [Bundler](http://bundler.io/) (Ruby Must Be Installed First!)  
```~$ gem install bundler```

* [Setup A Github Repository for Your Page](https://pages.github.com/)


####Setting Up Your Page####
---

1. Clone your Github Pages Repository to Your Computer
2. ```~$ cd <repository-location>```
3. Create a file in your repository called ```Gemfile```
4. Add these lines to your Gemfile:

```
source 'https://rubygems.org'
gem 'github-pages'
```

5. Run the command: ```~$ bundle install```
6. Pick a [Jekyll Theme](https://github.com/jekyll/jekyll/wiki/Themes)
7. Copy the source of the Jekyll Theme into your repository  


####Editing Your Page####
---
The main configuration will be in the ```_config.yml``` file. Fill in the options
with your information. Customization is different for each theme, but HTML and CSS files can
be configured to your liking.


####Testing Your Page####
---


To test your site in a way that will match with the github servers, run the command
```
~$ bundle exec jekyll serve```
in your repositories root directory. This will generate the page using jekyll and host
a local site that you can navigate to in your browser. Browse to
```
http://localhost:4000
```
This will let you preview your page before putting it online.

####Publish Your Page####
---
Push the contents of your repository to Github. If all goes well, your page should be online in a few minutes.
Extra setup information can be found [HERE](https://help.github.com/articles/using-jekyll-with-pages/).

---
