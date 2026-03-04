---
title: Creating This Website
date: 2026-03-02 21:47:00 -500
categories: [Website]
tags: [Website,Github,CI/CD,Automation]  # TAG names should always be lowercase
---

# What is Jekyll

[Jekyll](https://jekyllrb.com/) is a static site generator that transforms your plain text into beautiful static web sites and blogs. It can be use for a documentation site, a blog, an event site, or really any web site you like. It’s fast, secure, easy, and open source. 

Today, we’ll be installing and configuring Jekyll using the Chirpy theme. We configure the site, create some pages with markdown, automatically build it with a GitHub action and host it for FREE on GitHub pages.If you don’t want to host in the cloud, I show how to host it on your own server or even in Docker.


## How I created this Site

I started by following these instructions from TechnoTim: [TechnoTim Jekyll Doc Site](https://technotim.com/posts/jekyll-docs-site/)

Then I cloned the repo in my github account: [My Website Github Clone](https://github.com/Techwmaster/techwmaster.github.io)

Here is a link to the Chirpy Theme documentation: [Chirpy Documentation](https://chirpy.cotes.page/posts/getting-started/)

Here is more information about hosting your site for free on GitHub: [GitHub Page Documentation](https://docs.github.com/en/pages)

## Terminal Setup 
If you need help setting up your terminal on Windows, check out these two posts which will help you configure your terminal with WSL like mine




## Install Dependencies

```Shell
sudo apt get
sudo apt install ruby-full build-essential zlib1g-dev git
```
To avoid installing RubyGems packages as the root user:

If you are using **bash** (usually the default for most)

```Shell
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## To be continued...



