---
layout: post
title:  "A Style-Based Generator Architecture for Generative Adversarial Networks"
summary: "StyleGAN review"
author: sunwoo
date: '2021-04-02 16:10:00 +0900'
category: ['paper_study']
tags: jekyll
thumbnail: /assets/img/posts/paper_study/stylegan/stylegan.png
keywords: devlopr jekyll, how to use devlopr, devlopr, how to use devlopr-jekyll, devlopr-jekyll tutorial,best jekyll themes, multi categories and tags
usemathjax: false
permalink: /blog/stylegan-review/
---

## Introduction
<figure style="text-align: center">
	<img src="/assets/img/posts/paper_study/stylegan/pcgan.png" alt="pcgan.png"/>
	<figcaption>그림1. PCGAN으로 생성된 이미지 (from blog.lunit.io)</figcaption>
</figure>
위는 PCGAN으로 생성산 사람 얼굴 이미지이다.
```
---
category: ['jekyll', 'guides', 'sample_category']
---
```

Then to render this category using link and pages. All we need to do is,

1. Create a new file with [your_category_name].md inside categories folder.

2. Copy categories/sample_category.md file and replace the content in [your_category_name].md in that. (Please don't copy the code below its just sample, since it renders the jekyll syntax dynamically)

```jsx
---
layout: page
title: Guides
permalink: /blog/categories/your_category_name/
---

<h5> Posts by Category : {{ page.title }} </h5>

<div class="card">
{% for post in site.categories.your_category_name %}
 <li class="category-posts"><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</div>
```

Using the category, all the posts associated with the category will be listed on
`http://localhost:4000/blog/categories/your_category_name`


## Style-based Generator


## Style Mixing