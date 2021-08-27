---
layout: post
author: Ewelina Rupnik
image: images/diagram.png
toc: true
comments: true
hide: false
search_exclude: true
categories: [tutorial, article writing, markdown, jupyter, docx]
description: "A tutorial on notebook, markdown, Word doc article writing"
title: "How to publish a blog article"
---
# Introduction
All RFPT blogs are created using the [Github Pages](https://pages.github.com/)[^1] and to modify their content one needs a github account. There are at least two ways to publish a blog article. Here, we will present how to upload an article using the github web-interface. If you're more familiar with github, you may as well clone the repository locally, modify it as it fits, and push to the master branch via a pull request. 

You can download the blog templates from here:
- [Markdown template](https://github.com/rfpt-sfpt/tutorials/blob/master/assets/2021-08-24-Template.md)
- [Word Doc template](https://github.com/rfpt-sfpt/tutorials/blob/master/assets/2021-08-24-TemplateWord_v2.docx)

## Choose your blog category

The RFPT has several blogs. If you want to share information about a scientific or educational event (seminar, conference, etc.), submit your article to the [Education blog](https://rfpt-sfpt.github.io/education). If you want to write an article on your MSc or PhD thesis, choose the [Research blog](https://rfpt-sfpt.github.io/blog). Finally, if you want to publish a tutorial, go with the [Tutorials blog](https://rfpt-sfpt.github.io/tutorials). The corresponding github adresses, i.e., where to actual commits are submitted, are as follows:
* [Github Tutorials](https://github.com/rfpt-sfpt/tutorials)
* [Github Education](https://github.com/rfpt-sfpt/education)
* [Github Research](https://github.com/rfpt-sfpt/blog)

## File formats
An article can be submitted as a jupyter notebook, a markdown file or a Word file. Whatever the input file, a strict naming convention must be followed and it goes like this:
- `YYYY-MM-DD-*.ipynb` for notebooks
- `YYYY-MM-DD-*.md` for markdown files 
- `YYYY-MM-DD-*.docx`for Word docs

The `YYYY`, `MM` and `DD` correspond to the year, month and day of the publication (remember to separate them by a hyphen). The `*` symbol should be replaced with an arbitrary title.

## Location in the `github` folder structure

Depnding on the file format of your article, you should place it in their corresponding folders. If you've written 
- a notebook article, place it inside the `_notebooks` folder, 
- a markdown article, place it inside the `_posts` folder, and
- a Word doc article, place it inside the `_word` folder.

In the following figure, the folders are marked with red, green and blue rectangles, respectively:

![]({{ site.baseurl }}/images/github-folder-structure-marked_thumb.png "Place your article in the corresponding folder (notebook, post, or word).")

# Write or upload and submit

## Markdown article
> Please take a look at [this post](https://rfpt-sfpt.github.io/education/markdown/2020/01/14/test-markdown-post.html) to learn some basic markdown functions such as defining a list/table, or embedding an image or even a piece of code in your post! 

You're now ready to create or upload your article. Below find the instructions on how to succesfully submit your post.


1. Go to the github address corresponding to your blog 
```yaml
   Tutorials : https://github.com/rfpt-sfpt/tutorials
   Education : https://github.com/rfpt-sfpt/education
   Research  : https://github.com/rfpt-sfpt/blog
```
2. Upload an existing file or create a new one
3. Include `front matter` to describe the metadata of the article such as author, title, description, tags, image. You're highly encouraged to include an image, which   will be displayed on the main page, next to your article. Do not forget to upload the image file inside the `images` directory prior to submitting your post. 
4. Write the content of your article using the [markdown language](https://guides.github.com/features/mastering-markdown/) 
5. Submit the article with the `Commit changes` button. This will create the so-called `pull request` that one of RFPT moderators will need to confirm and merge with the blog content.

The above instructions are summarised in the figure below:

![]({{ site.baseurl }}/images/tutorial_write_blog.png "The instructions in **picture**")

## Notebook article

If you created a `ipnyb` notebook file, [fastpages](https://github.com/fastai/fastpages) allow to automatically convert it to its blog-like version. It's sufficient to upload your notebook in the `_notebook` folder, and follow the `YYY-MM-DD-*.ipynb` naming convention. Please refer to [this examplar post](https://rfpt-sfpt.github.io/tutorials/jupyter/2020/02/20/test.html) for more information.

## Word article

You can publish an article using the Word docx file, however, it does not seem to be the recommended way of interacting with the fastpages blog. Follow [this tutorial](https://fastpages.fast.ai/2020/01/01/Microsoft-Word-Example-Post.html) for more information.

# Other references

- [Writing Blogs With Jupyter](https://github.com/fastai/fastpages#writing-blog-posts-with-jupyter)

- [Writing Blogs With Markdown](https://github.com/fastai/fastpages#writing-blog-posts-with-markdown) 

- [Writing Blog Posts With Word](https://github.com/fastai/fastpages#writing-blog-posts-with-microsoft-word)

[^1]: The blog content was generated with the help of the ingenious [fastpages](https://github.com/fastai/fastpages) blogging platform.
