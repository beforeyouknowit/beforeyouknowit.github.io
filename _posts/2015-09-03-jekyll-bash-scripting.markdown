---
layout: post
title: "Jekyll Bash Scripting"
author: Ashley Theiss
date: 2015-09-03 13:34:52
tags: 
- HERE
img: HERE.jpg
thumb: HERE.jpg
summary: Find out Ashley's tips and scripts for how to make your life with Jekyll and the Terminal completely streamlined.
---

While I was in the process of building this Jekyll blog, and several other Jekyll-based sites I have on the go, I decided that I needed a simple, reliable, and consistent way of writing and posting new content onto each respective site.

After extensive research (i.e. by Googling, browsing [Github](https://www.github.com/) and [StackOverflow](https://stackoverflow.com/), and asking friends in the office, namely Arvinder and [Phil](https://github.com/pjama),) I've managed to assemble a few Bash scripts to help make life with Jekyll much easier.

I wound up developing 3 very similar scripts. The first one, `jnpost`, prompts me for the Jekyll blog post title, then formats the date and YAML frontmatter, and opens up the new `.markdown` file for me in [Sublime Text](https://www.sublimetext.com/).

From there, I can simply write the body of my post in Markdown, `Cmd + S` to save it to disk, then return to my terminal, `git add .` then `git commit -m "Commit message"` then `git push` and it's on the web.

Here's what the `jnpost` script looks like:

<script src="https://gist.github.com/beforeyouknowit/2707b0705338873b9b07.js"></script>

The other two similar scripts are `jnproj` for creating new Project posts on other sites (such as ones that have Portfolio pages, etc.) and the other is `jndraft` for writing draft posts. The latter requires a `_drafts` folder to be in the Jekyll site folder, and it's presumed to be included in the `.gitignore` so that it doesn't get picked up by Git. (I figured that I might want to keep a pile of unfinished drafts on the back burner, and just store them locally before turning them into formal Posts.)

I can share those other two scripts too, but since they're even more situationally-customized I doubt they'd be useful for as many Jekyll bloggers and developers as my `jnpost` script.

Just leave a comment below if you need help with these, or if you'd like me to share these two bonus scripts publically too.

Enjoy!