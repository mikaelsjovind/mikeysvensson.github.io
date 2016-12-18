---
title: "Display images in a folder with Jekyll"
date: 2016-12-18
---

![Up on the hill](/images/2016-12-13-the-hill.jpeg)

Jekyll has a site variable called [site.static_files](http://jekyllrb.com/docs/static-files/). A static file is a file that does not contain any YAML front matter. These include images, PDFs, and other un-rendered content.

You can use this variable to display images you have in a specific folder. In this example I iterate over all files and only output the ones with /image/ in the file path. 

{% raw %} 
	{% for file in site.static_files %}
		{% if file.path contains '/images/' %}
			<div><img src="{{ file.path }}"/></div>
		{% endif %}
	{% endfor %}
{% endraw %}