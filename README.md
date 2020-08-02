# **Beacon's Eyes**

Design by Ella.

## About

This is the repo for Ella's design work. To view the site visit [http://beaconseyes.com](beaconseyes.com).

This site is hosted on github pages and runs using [jekyll](https://jekyllrb.com/), a static site generator.

### Updating content
Visit any .md file and modify its content using [markdown syntax](https://guides.github.com/features/mastering-markdown/). There may be comments in the file saying not to edit that file, but if there are they should also tell you what file you _should_ be editing. If there isn't you have permission to beat Yo gently with a stick. Some basic guides:

- `assets` is the folder where you can put images. Make sure to give them descriptive names. Don't edit the .scss file in this folder, it's necessary for the theme to work on GitHub Pages.
- `_config.yml` has some settings like the site slogan and email address.
- `README.md` is the page that has all this info :)

These folders are for the site design and layout: if you're just editing content it's safe to ignore them:

- `_includes` holds partial page components for the site layout.
- `_layouts` holds pages templates. It's what one would edit to change how all the pages look.
- `_sass` contains the stylesheets - things like colour, fonts, etc. If you need to edit it, only edit the custom.scss file. Don't edit any of the others, they're from a jekyll theme and overriding them would make it hard to update the theme later without losing your content.

Files it's probably safe to ignore that do technical stuff for the site:

- `.gitignore` prevents people who use git on their computers from adding the wrong files to this repo by accident.
- `CNAME` is used to set the domain name, so don't change it unless you're moving the site to a different URL.
- `Gemfile` and `Gemfile.lock` are files that are used by jekyll, the framework that generates the site, to fetch certain bits of software it needs to generate the site. Leave these where they are and don't change them unless told to ;)

#### Adding new pages
Always copy an existing .md file as it makes things a little easier. You'll see the top of each page has some info between two sets of three dashes, like this:

```yml
---
layout: page
title: About
featured-image: assets/ella.jpg
shadowed-image: true
---
```

Generally, you'll want **layout** to be `page`, but other options are `home` or `post` - and we can add more layout types if you need them later on.  

**title** is hopefully reasonably straightforward :)

**featured-image** if you would like the page to have an image on the left, put the image in the `assets` folder and then put the link to the file in the featured-image folder.

**shadowed-image** this will automatically add a box shadow behind the image. set to `true` if you want to see the shadow, and leave it out or set it to `false` if you don't want it. See the about page for an example.

**link-title** if you want the link to your page in the nav bar to be different to your page title on the page itself (e.g. perhaps you want the navbar to say "about" but you want the page's header to say "about me"), then set link-title.

**link-url** if you want the link in the homepage navbar to link to outside your site, put its URL here. See portfolio.md for an example.

**show-in-nav** if you want the page to show in the navbar, set this to true or leave it out entirely. IF you don't want the page to show, set it to `false`.

**price-list** set to true if you want to have purple boxes with prices in them. To make a price box, you'll then need to use a level two heading and a list, e.g.:

```markdown
## Single-Sided, A5
- $24.99
- Up to 3 hours work
- 1 hour of revision
```

This will create a purple box with prices, but won't do so for headers that are first or third level. See flyer-design.html for an example.

### Credits

Site design by Ella, site code by [Yo Yehudi](http://github.com/yochannah)
