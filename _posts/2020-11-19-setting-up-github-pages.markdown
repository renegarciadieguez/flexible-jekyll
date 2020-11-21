---
layout: post
title: Setting up GitHub Pages
date: 2020-11-19 20:40:20 -0800
description: This pages describes the steps to setup a GitHub pages site.
img: github-pages.jpg
fig-caption: GitHub Pages
tags: [GitHub, Pages, First]
---
This first post will describe the steps required to setup and customize the a new GitHub Pages site using the theme
[flexible-jekyll](https://github.com/artemsheludko/flexible-jekyll).

## Fork the repo ##
After forking the repo you'll need to go to your version of the repo's settings and publish the master branch. GitHub
will then show you the url for the site. In my case, https://renegarciadieguez.github.io/flexible-jekyll/.

![Settings](../assets/img/settings.jpg)

Wait a few minutes. GitHub needs to build and deploy the pages.

## Clean up ##
Before customizing the site, make sure to add the relevant directories for your favorite IDE or code editor to the
`.gitignore` file (in my case, `.idea/` for all the Jetbrains IDEs) and remove any files you won't need... such as any
previously checked in `.DS_Store` files. Here's a handy command to find and delete those:
```zsh
find <LOCAL_REPO_DIRECTORY> -name '.DS_Store' -type f -delete
```
## Customizing the site's configuration ##
The `_config.yml` file contains a number of site-wide settings, including the site's title, description, and the author
information. Start the customization of your site there. 

## Making a post ##
The `_posts` directory contains a series of `.markdown` files. Delete all the files except for one. I'm my case, the one
I kept was renamed to `_posts/2020-11-19-setting-up-github-pages.markdown` and it resulted in the post you're
[reading](https://renegarciadieguez.github.io/flexible-jekyll/setting-up-github-pages/).

## Layout ##
The `_layouts` directory contains [Liquid](https://jekyllrb.com/docs/step-by-step/02-liquid/) templates. That's where
you will be able to find html components used to frame the site. For example I removed the "Contact Me" section
completely, but you can add and update the icons or add more relevant information. 

## Finally ##
### GiHub ###
Have a look at the first few commits after the fork, e.g.
[`5b21c17`](https://github.com/renegarciadieguez/flexible-jekyll/commit/5b21c178a91f44a181e02a81733c5957e12b1091),
[`d1c1772`](https://github.com/renegarciadieguez/flexible-jekyll/commit/d1c17727a080bb0456fb1ee02ecb0319d5badb7a),
[`219e92e`](https://github.com/renegarciadieguez/flexible-jekyll/commit/219e92eef6acda9df5438e9b38795116caf03cfc),
[`2b04b8c`](https://github.com/renegarciadieguez/flexible-jekyll/commit/2b04b8c663c098970a07523669ff334e939beb24),
[`65ad410`](https://github.com/renegarciadieguez/flexible-jekyll/commit/65ad4104c78f97d2d21f139d085b1c9d25e29b46),
[`cfbbff2`](https://github.com/renegarciadieguez/flexible-jekyll/commit/cfbbff25fcc3c9a6606a7be3a4417764ddc26ee8),
[`1fcd077`](https://github.com/renegarciadieguez/flexible-jekyll/commit/1fcd0775562a1bc4547658924eb9fae10a26bc81)
to see more details of how the theme was initially configured.

### More Documentation ###
- See [pages.github.com](https://pages.github.com)
- See [jekyllrb.com](https://jekyllrb.com)

---
Cheers!
