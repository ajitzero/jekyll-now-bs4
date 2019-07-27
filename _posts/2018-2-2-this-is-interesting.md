---
layout: post
title: With syntax highlighting
author: Ajit
updated: 2019-7-27 12:00:00 +0530
og-image: assets/images/config.png
categories:
  - web
---

Check this one for an example on using OpenGraph images per post.
 
Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

{% highlight javascript %}
const test1 = () => {
  console.log("Syntax highlighting");
};

const test2 = () => {
  console.log("Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus doloribus a atque corporis quisquam. Quidem, enim accusantium quas voluptates molestiae quaerat accusamus saepe possimus eum iste? Quo voluptatem minus neque?");
};
{% endhighlight %}

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.