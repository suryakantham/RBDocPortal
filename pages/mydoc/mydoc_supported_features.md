---
title: Supported features
tags:
  - getting_started
keywords: "features, capabilities, scalability, multichannel output, dita, hats, comparison, benefits"
last_updated: "February, 2018"
summary: "Learn more about the Rollbase features"
published: true
sidebar: mydoc_sidebar
permalink: mydoc_supported_features.html
folder: mydoc
datatable: true
---


## Creating tooltips
Because this theme is built on Bootstrap, you can simply use a specific attribute on an element to insert a tooltip.

Suppose you have a glossary.yml file inside your \_data folder. You could pull in that glossary definition like this:

{% raw %}
```html
<a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.jekyll_platform}}">Jekyll</a> is my favorite tool for building websites.
```
{% endraw %}

This renders to the following:

<a href="#" data-toggle="tooltip" data-original-title="{{site.data.glossary.jekyll_platform}}">Jekyll</a> is my favorite tool for building websites.


## Formatted Information

You can insert a tip, note, warning, or important alert simply by using these tags.


```liquid
{% raw %}{% include note.html content="Add your note here." %}{% endraw %}
```


```liquid
{% raw %}{% include tip.html content="Add your tip here." %}{% endraw %}
```


```liquid
{% raw %}{% include important.html content="Add your important info here." %}{% endraw %}
```


{% raw %}
```liquid
{% include warning.html content="Add your warning here." %}
```
{% endraw %}

Here's the result:

{% include note.html content="Add your note here." %}

{% include tip.html content="Here's my tip." %}

{% include important.html content="This information is very important." %}

{% include warning.html content="If you overlook, this session may get killed." %}

The color scheme is the default colors from Bootstrap. You can modify the icons or colors as needed.

## Nav tabs

The following is a demo of a navtab. Refresh your page to see the tab you selected remain active.

<ul id="profileTabs" class="nav nav-tabs">
    <li class="active"><a class="noCrossRef" href="#control" data-toggle="tab">Control Panel</a></li>
    <li><a class="noCrossRef" href="#components" data-toggle="tab">Components</a></li>
    <li><a class="noCrossRef" href="#shared" data-toggle="tab">Shared Properties</a></li>
</ul>
  <div class="tab-content">
<div role="tabpanel" class="tab-pane active" id="control" markdown="1">

## Control Panel

From the Control Panel, you can perform the following actions:
 1. Update your Rollbase license details
 2. Download Usage Report
 3. Re-create Lucene index
      * Reset the Master cache
      * Configure the email server, authentication details, and Google integration
 4. Modify the details of field groups, list items, security and service levels and default cards



> View and modify the code templates pertaining to Java, Node and PHP.
</div>

<div role="tabpanel" class="tab-pane" id="components">
    <h2>Components</h2>
    <p>Displays the list of Rollbase components (such as server name and details) for view and edit with component type (such as MASTER, PROD, STORAGE, SEARCH), properties (Name and Path), Stats (number of customers and sessions for each component), Host Name (IP address), Time Running (duration), and Running Jobs information.</p></div>

<div role="tabpanel" class="tab-pane" id="shared">
    <h2>Shared Properties</h2>
    <p>Displays the list of Shared Properties by category such as General, Customize and Limits. You can view or configure the properties from here. Backend changes are no longer needed.</p>
</div>
</div>

## Download Sample files

You can see an example of the finished product here:

<a target="\_blank" class="noCrossRef" href="{{ "pdf/my_markdown_cheatsheet.pdf"}}"><button type="button" class="btn btn-default" aria-label="Left Align"><span class="glyphicon glyphicon-download-alt" aria-hidden="true"></span> PDF Download</button></a>


## Vimeo player

{% include vimeoPlayer.html id=252930854 %}

## HTML Tables {#htmltables}

If you need a more sophisticated table syntax, use HTML syntax for the table. Although you're using HTML, you can use Markdown inside the table cells by adding `markdown="span"` as an attribute for the `td` tag, as shown in the following table. You can also control the column widths.

```html
<table>
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">First column **fields**</td>
<td markdown="span">Some descriptive text. This is a markdown link to [Google](http://google.com). Or see [some link][mydoc_tags].</td>
</tr>
<tr>
<td markdown="span">Second column **fields**</td>
<td markdown="span">Some more descriptive text.
</td>
</tr>
</tbody>
</table>
```

**Result:**
<table>
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">First column **fields**</td>
<td markdown="span">Some descriptive text. This is a markdown link to [Google](http://google.com). Or see [some link][mydoc_tags].</td>
</tr>
<tr>
<td markdown="span">Second column **fields**</td>
<td markdown="span">Some more descriptive text.
</td>
</tr>
</tbody>
</table>

## jQuery DataTables


<div class="datatable-begin"></div>


Property        | Description                                                                                           | Category | Y/N
---------------------- | ----------------------------------------------------------------------------------------------------- | -------- | ---
HostName               | Host name of your master server.                                                                      | Platform | Y   
IsSecureServer         | Determines the security protocol for all communications between your system and the web server.       | General  | Y   
Kiwis                  | A small, hairy-skinned sweet fruit with green-colored insides and seeds.                              | Fruit    | N   
Oranges                | A spherical, orange-colored sweet fruit commonly grown in Florida and California.                     | Fruit    | N   
Cat                    | A small, furry and soft animal that can be domesticated and makes a sound like **Meow**.              | Animal   | Y   
Tree                   | A very big plant.                                                                                     | Fruit    | N
HostName               | Host name of your master server.                                                                      | Platform | Y   
IsSecureServer         | Determines the security protocol for all communications between your system and the web server.       | General  | Y   
Kiwis                  | A small, hairy-skinned sweet fruit with green-colored insides and seeds.                              | Fruit    | N   
Oranges                | A spherical, orange-colored sweet fruit commonly grown in Florida and California.                     | Fruit    | N   
Dog                    | A wolf like animal that can be domesticated and barks emitting a sound like **Bhow-How**.             | Animal   | Y   
Plant                  | A very small tree.                                                                                    | Fruit    | N
Oranges                | A spherical, orange-colored sweet fruit commonly grown in Florida and California.                     | Fruit    | N   
Cat                    | A small, furry and soft animal that makes a sound like **Meow**.                                      | Animal   | Y   
Tree                   | A very big plant.                                                                                     | Fruit    | N
HostName               | Host name of your master server.                                                                      | Platform | Y   
IsSecureServer         | Determines the security protocol for all communications between your system and the web server.       | General  | Y   
Kiwis                  | A small, hairy-skinned sweet fruit with green-colored insides and seeds.                              | Fruit    | N   
Oranges                | A spherical, orange-colored sweet fruit commonly grown in Florida and California.                     | Fruit    | N   
Dog                    | A wolf like animal that can be domesticated and barks emitting a sound like **Bhow-How**.             | Animal   | Y   
Plant                  | A very small tree.                                                                                    | Fruit    | N

<div class="datatable-end"></div>

Notice a few features:

* You can keyword search the table. When you type a word, the table filters to match your word.
* You can sort the column order.
* You can page the results so that you show only a certain number of values on the first page and then require users to click next to see more entries.

{% include note.html content=" Try to keep the columns to 3 or 4 columns only. If you add 5+ columns, your table may create horizontal scrolling with the theme. Additionally, keep the column heading titles short." %}

{% include links.html %}
