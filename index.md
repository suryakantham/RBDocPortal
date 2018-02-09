---
title: "Getting Started"
keywords: sample homepage
tags: [getting_started]
sidebar: mydoc_sidebar
permalink: index.html
summary: This topic provides Rollbase overview, insights on using Jekyll and Git Markdown.
toc: false
---

## About Rollbase

Welcome to Progress® Rollbase® a web-based platform for creating, customizing and distributing applications. Rollbase applications run in an integrated online environment and share a common security model, data model and user interface. Rollbase exemplifies Platform-as-a-Service (PaaS). There is no hardware or software to buy or install, both developers and end-users access Rollbase using a web browser. Rollbase allows you to focus on creating business value for users rather than on the expensive, complex and time-consuming tasks of managing software and infrastructure.

{% include inline_image.html file="rbinterface.png" alt="Rollbase Interface" %}


{% include note.html content="If you want to first create and design workflows, see [Visual Workflow Designer][mydoc_about]" %}




To quickly learn and master the Git Markdown syntax, visit [Cheatsheet on Git Markdown Syntax](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)



This is a code block:

```
var d1 = new Date('2/2/2014');
var d2 = new Date('4/2/2014');
var arr = rbv_api.selectQuery(
"SELECT id, name FROM a1 WHERE createdAt BETWEEN ? AND ?", 100, d1, d2);
rbv_api.printArr(arr);
```


{% include links.html %}
