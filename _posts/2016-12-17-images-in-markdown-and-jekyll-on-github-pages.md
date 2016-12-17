---
layout: post
title: "Images in Markdown and Jekyll on Github Pages"
date: 2016-12-17
---

![Walking bridge to Liseberg](/images/2016-12-04-jul-pa-liseberg-bridge.jpg)

The above image was put into place by the following steps.

1. Add a folder in your root called /images
2. Upload an image
3. Create a new post
4. Reference the images with the following Markdown syntax

`![Walking bridge to Liseberg](/images/2016-12-04-jul-pa-liseberg-bridge.jpg)`

Note that you have to have a /images/ and not a relative images/ reference. Also make sure to write .JPG if the file has capital letters in .JPG.

You can also use HTML if you want to specify more attributes, such as width.

`<img src="/images/2016-12-04-jul-pa-liseberg-bridge.jpg" width="100%" alt="Walking bridge to Liseberg">`

I added this to my CSS instead.

`img { width: 100%; }`
