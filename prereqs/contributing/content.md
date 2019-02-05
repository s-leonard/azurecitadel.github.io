---
title: Structuring Your Content
date: 2019-01-18
author: Richard Cheney
comments: true
hidden: true
published: true
permalink: /contributing/content/
header:
  overlay_image: /images/site/main.png
excerpt: Site content
sidebar:
  nav: "contributing"
---

# Where should new files go?

The standard content from the contributors is held in the category folders, e.g.:

```text
📁 automation/
📁 cloud-native/
📁 data-ai/
📁 devops/
📁 fundamentals/
📁 infra/
📁 iot/
📁 security/
📁 web/
```

These folders are referenced by the `/_data/categories.yml` file. You won't need to change this file.  (If you think there should be a change to the categories then let us know in the comments.)

The **_data** directory also contains YAML format files to manage the authors and custom navigation. We will cover these later in the guide.

# Out of bounds

The following areas are out of scope for contributions and may be ignored. Feel free to [skip forward](#style).

The other *_dir* areas contain the theme files and Jekyll build controls. These are used in combination with files in the root of the repo (such as _config.yml) to control the automated site generation.

When files are generated by Jekyll, they are placed in **_site**.  This is one of the many files and directories ignored by Git via the **.gitignore** file so you will not see this in your GitHub fork.

The posts used for the News section are held in **_posts**.  Notice the naming convention, which is mandated and ensures the posts are ordered chronologically.  The _posts area is

There are a number of legacy folders that may also be ignored:

```text
📁 guides/
📁 labs/
📁 workshops/
```

Please do not create content in these folders.

> (For the record, the html redirect files in here were created locally using the /_redirects.htaccess file and the /_plugins/pageless_redirects.rb plugin from <https://github.com/nquinlan/jekyll-pageless-redirects>. The generated HTML redirects were then manually copied from the _site folder into the root as GitPages does not support custom plugins.)

# Style

This a community site for technical Azure users, so your content should be geared for them.

Keep the text professional, concise and clear.

Make full use of headers links, lists and pictures to make the content easy to digest.

# Navigation

The H1 and H2 headers on each page will be used to generate the navigation pane on the right.  Keep the number of headers sensible so that the navigation pane doesn't become too long for standard screen sizes.

# Centralised media

We'll ignore the page specific media for the moment.

There is an **/images** folder that hosts the images used for the main site pages, the category pages, and the author pictures.

The **/images/header** folder holds the banner photos used for the title backgrounds.

The **/images/teaser** folder contains the smaller images used in the category grids.

These images get reused on multiple pages, which is why they are kept centrally.

# Next

The following page goes through single page content using an example template and gives an opportunity to go through the recommended structure.

[◄ Authors](../authors){: .btn .btn--inverse} [▲ Index](../#index){: .btn .btn--inverse} [Single Page ►](../singlepage){: .btn .btn--primary}