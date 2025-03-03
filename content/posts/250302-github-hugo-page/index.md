+++
title = "Quick Github Hugo Page"
date = "2025-03-03T09:31:36+01:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "Viking Cat"
authorTwitter = "" #do not include @
cover = ""
tags = ["post", "github", "hugo"]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
+++

Did you know that you can easily host a simple website for free? [Github](https://github.com/) has something called [Pages](https://pages.github.com/) (***[documentation](https://docs.github.com/en/pages)***)that allows you to write content in [Markdown](https://en.wikipedia.org/wiki/Markdown) and then automatically convert it into a static page with [Jekyll](https://jekyllrb.com/). 

But it goes further then that, you can write and present regular HTML or use another website generator with the help of Githubs pipeline system called Actions

Hugo is a recent static site generator (***aka SSG***) written in Golang. This tool makes it easy to create and maintain websites that are less dynamic and more static. Greate examples are blogs, documentation, marketing websites. A big benefit is that static content is fast by nature and more reliable.



This guide assume that you already know how to work with Git and have a general experience with development in general.

1. Install Hugo by following the official [Hugo Quick Start Guide](https://gohugo.io/getting-started/quick-start/)

2. Set up a repo your way for the github hugo page. I ended up calling the repo "web" for "website".

3. Push your hugo page to github

## Setup github pages for the repository

1. Login to github
2. Go to your repository
3. Settings -> Pages 
4. Under **Build and deployment** change **source** from ***Deploy from branch*** to ***Github actions***
5. Select the **browse all workflows** link
6. Search for **hugo**
7. Press the **configure** button
8. Press the **Commit changes** button on the right side
9. You will be presented with a popup window where you can add information to the commit. Press the **Commit changes** button when you are finished.

The last step in this list will add ***./.github/workflows/hugo.yaml*** to your project repository and automatically start the first build.


