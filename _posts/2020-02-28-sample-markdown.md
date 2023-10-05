---
layout: post
title: Linked Fusion
subtitle: Interpretation of Observations
---

<blockquote style="text-align:center;">“GOAL: retrieve
the smallest building blocks from the observations that make up a scene.”</blockquote>

<div style="text-align: justify">

In the context of LinkedFusion, the goal is to extract the smallest building blocks from observations that compose a scene. These building blocks, which may not necessarily be structural elements, represent the minimal segments required for coherent objects. This mathematical problem involves maximizing the conditional probability of a set of segmentations based on feature inputs, such as XYZ coordinates and color information for point clouds, or pixel values for images.

![Segmentation](../assets/img/segmentation.PNG)

Currently, each modality (point clouds and images) is processed independently, leading to specific interpretation models for each. While this approach is common, it has limitations, especially in domains like construction, where objects vary in texture and geometric features. Achieving market adoption rates of around 90% necessitates combining these approaches, prompting the key question of how to fuse them effectively.

</div>

{: .box-success}
This is a demo post to show you how to write blog posts with markdown.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](https://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/tables/etc.<br/>I also encourage you to look at the [code that created this post](https://raw.githubusercontent.com/daattali/beautiful-jekyll/master/_posts/2020-02-28-sample-markdown.md) to learn some more advanced tips about using markdown in Beautiful Jekyll.

**Here is some bold text**

## Here is a secondary heading

[This is a link to a different site](https://deanattali.com/) and [this is a link to a section inside this page](#local-urls).

Here's a table:

| Number | Next number | Previous number |
| :------- | :------------ | :---------------- |
| Five   | Six         | Four            |
| Ten    | Eleven      | Nine            |
| Seven  | Eight       | Six             |
| Two    | Three       | One             |

How about a yummy crepe?

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg)

It can also be centered!

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes

You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

## Local URLs in project sites {#local-urls}

When hosting a *project site* on GitHub Pages (for example, `https://USERNAME.github.io/MyProject`), URLs that begin with `/` and refer to local files may not work correctly due to how the root URL (`/`) is interpreted by GitHub Pages. You can read more about it [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). To demonstrate the issue, the following local image will be broken **if your site is a project site:**

![Crepe](/assets/img/crepe.jpg)

If the above image is broken, then you'll need to follow the instructions [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). Here is proof that it can be fixed:

![Crepe]({{ '/assets/img/crepe.jpg' | relative_url }})

