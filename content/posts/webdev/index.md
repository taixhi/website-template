---
title: An introduction to web development for normies
date: 2021-10-31T00:00:00-05:00
marp: true
description: Learn how to build and host your own website for free!
date: 2021-10-31T02:09:12-05:00
theme: default
tags: [tutorial, dev]
---
<!-- headingDivider: 1 -->

Amherst College
October 31st 2022

Check out the slides [here](slides.html)


Today: Learn how to build and host a website

Not any website, but a **personal** website.

# What do personal websites look like?
- Some examples  
	- [Gwern](https://www.gwern.net/)  
	- [Andy](https://andymatuschak.org/)  
	- [Nick](http://nickcammarata.com/)  
- Some student examples  
	- [Daniel](https://danielnjoo.notion.site/)  
	- [Sawyer](https://sawyerpollard.com/)  
	- [Alex](https://www.delfran.co/about/)  
	- [Taichi](https://taichikato.com/photography)  

# I see two primary goals: **selling/sharing**
- *Sell* something (your image, service or yourself)  
- *Host* Knowledge (share your knowledge, contribute to a conversation, create sharable and persisting piece of knowledge)  

# Why **you** should have a website:
- Ownership: **Own** your online identity and distribution. You won't be deplatformed.
- Customizability: Limitless playground that you can customize and showcase to the world
- Opportunities: Build credibility and showcase skill on your own terms
It's also a lot of fun, and somewhat liberating.
...

# Why **you** should have a website:
<blockquote class="twitter-tweet"><p lang="en" dir="ltr">“it’s a politically meaningful act to have a personal website”</p>&mdash; Visa’s Treacherous Talismans (@visakanv) <a href="https://twitter.com/visakanv/status/1571851741553102848?ref_src=twsrc%5Etfw">September 19, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

# Hopefully, you're convinced that it's good to have a website


# What are the requirements?
Requirements: Minimum  
- No corporate branding  
- 99.9% up-time  
- No-code solution to host  
- Portability  
- Customizability  
- Ability to serve a single page 
- Cheap!

# What are the requirements? (2)
 Requirements: Optional/nice to have  
- Blogging capacity  
- Content management system (CMS)  
- Custom domain  
- Nice design  
- Dynamic content  
- Maybe integration with notes?  
- ecommerce?  
- custom email  


# Your options
- Hugo with Github (free + custom domain)  
- Notion (free, but expensive with custom domains)  
- Squarespace (expensive ~$16/mo...tf?)  
- Carrd (free, but $20/yr to host with custom domain)  
- [Self-host an html file through the college (free!)](https://www.amherst.edu/offices/it/academic-technology-services/tools/web/web-hosting)  

# Your options: illustrated
![width:20cm](https://github.com/taixhi/website-template/raw/main/hosting.png)  
*Today: Github pages*

# Demo Time!
# Set up Github
- Create a Github account  
- Create a repository from [my template](https://github.com/taixhi/website-template)  
- Name your project `<user>.github.io`  
- After the repository gets populated with files, navigate to settings  
	- Select “pages” on the left side panel  
	- Go to branch—select `gh-pages`, and click save  
- After a while, refresh the settings/pages page, and the link to your website should show up.  
- Tip: to learn what's happening under the hood, you can learn more about Hugo and Github pages below:  
	- [Hugo](https://gohugo.io/)  
	- [Github Pages](https://pages.github.com/)  
	- [Host Hugo on GitHub](https://gohugo.io/hosting-and-deployment/hosting-on-github/)  


# Required modification to the template
- `config.toml`: Update `baseURL` to your domain name  
- `content/_index.md`: To edit the main text on the main page (written in [Markdown](https://www.markdownguide.org/cheat-sheet/) format)  
- `content/posts/xx.md`: This is where your `posts` live.  


# Next steps
- Edit the layout in `themes/archie/layouts/index.html` to include a profile picture. This file is written in `html` with some `Go` to allow for templating.  
- Change the design through editing `themes/archie/assets/css/main.css`. The file is written in a format called `CSS`, which you can learn more about here: https://web.dev/learn/css/  
- Use a custom domain (recommend: use `namecheap.com`. Make sure to update domain name in the `config.toml` after, and set up custom domain in the `pages` setting)  
- Set up Google Analystics to track users and pageviews (edit `themes/archie/layouts/partials/header.html`) to input the google analytics tag  

# Next steps (2)
- Get git installed: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git  
- Install Hugo (may need to install `Homebrew` if on mac, as well): https://gohugo.io/getting-started/installing  
- `Clone` your website to your computer: https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository  
- Navigate to your repository on the Terminal (In macOS, open `Terminal` and run `cd` space `/path/to/your_website_folder`) 

# Extension
- Use a CMS (Content management service) to manage media through a web interface, instead of editing files in Github  
- Set up a form on the website  
- Create animations with CSS and JS  
- Customize the website with CSS  
- ...and more!  
