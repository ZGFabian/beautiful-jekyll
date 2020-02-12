---
layout: post
title: Formating demo
subtitle: Styling pages using markdown, html and liquid formatting tags
# gh-repo: daattali/beautiful-jekyll
# gh-badge: [star, fork, follow]
tags: [markdown, html, css, liquid, todo]
# comments: true
lang: en
common-js: "https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"
---
><img src="/img/20-02-10-formatting/markdown_small.png"
>      alt="markdown_logo"
>      style="float: right; margin-right: 10px; margin-left: 15px; zoom: 80%;" />
>**"Markdown is not a replacement for HTML, or even close to it. Its syntax is very small, corresponding only to a very small subset of HTML tags. The idea is not to create a syntax that makes it easier to insert HTML tags. In my opinion, HTML tags are already easy to insert. The idea for Markdown is to make it easy to read, write, and edit prose. HTML is a publishing format; Markdown is a writing format. Thus, Markdown’s formatting syntax only addresses issues that can be conveyed in plain text.   
>For any markup that is not covered by Markdown’s syntax, you simply use HTML itself. There’s no need to preface it or delimit it to indicate that you’re switching from Markdown to HTML; you just use the tags."**


-- [John Gruber](https://daringfireball.net/projects/markdown/syntax#philosophy) the inventor of the Markdown markup language. 

# Header 1

## Here is a secondary heading

Here's a useless (& ugly) .md table:

	| Number | Next number | Previous number |
	| :------ |:--- | :--- |
	| Five | Six | Four |
	| Ten | Eleven | Nine |
	| Seven | Eight | Six |
	| Two | Three | One |

Which is rendered to .html like this:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |

Not bad, but you may want to pretty raw format:

	|  Number | Next number | Previous number |
	|---------|-------------|-----------------|
	| Five    | Six         | Four            |
	| Ten     | Eleven      | Nine            |
	| Seven   | Eight       | Six             |
	| Two     | Three       | One             |


<div class="alert alert-success">
  <i class="fa-lightbulb"></i> <strong>Tip:</strong> Creating tables in markdown can be a pain without advanced an editor like Sublime Text, Vim or Emacs. In such situations one can try the <a href="https://www.tablesgenerator.com/markdown_tables">Markdown Tables Generator</a>. I am using [Table Editor plugin](https://github.com/SublimeText-Markdown/TableEditor) with Sublime. 
</div>

{: .box-note}
**Note:** You can add html tags (center, kbg, etc) inside a markdown text. 


A markdown picture resized with custom css in URI

![BlaBlaBla](/img/site/blabla_av_orange.png#thumbnail2)

Images can also be centered like this `![BlaBlaBla](/PATH/){: .center-block :}`

![BlaBlaBla](/img/site/blabla_av_white_bg.png#thumbnail){: .center-block :}


<div class="container"> 
<img src="/img/20-02-10-formatting/markdown_small.png" alt="markdown_logo"
      style="float: right; margin-right: 10px; margin-left: 15px; zoom: 80%;" /> 
</div>

<br>
Here's a markdown code chunk with an html image aligned:

<img align="right" src="/img/site/blabla_av_orange.png" width="50">
~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is some R code with syntax highlighting:

<img align="right" src="/img/site/blabla_av_white_bg.png" width="50">
```r
setwd(~) 
text <- readLines("text.txt")
head(text, 50)

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
**Note:** This is a notification box. `{: .box-note}`

### Warning

{: .box-warning}
**Warning:** This is a warning box. `{: .box-warning}`

### Error

{: .box-error}
**Error:** This is an error box. `{: .box-error}`

## Icons

<div class="alert alert-info" role="alert"><i class="fa fa-exclamation-circle"></i>
  This is a **info** alert with <a href="https://www.w3schools.com/icons/bootstrap_icons_glyphicons.asp" class="alert-link">an example link</a>.
</div>
<div class="container">
  <h2>Search Glyph</h2>
  <p>Search icon: <span class="glyphicon glyphicon-search"></span></p>    
  <p>Search icon as a link:
    <a href="#">
      <span class="glyphicon glyphicon-search"></span>
    </a>
  </p>
  <p>Search icon on a button:
    <button type="button" class="btn btn-default btn-sm">
      <span class="glyphicon glyphicon-search"></span> Search 
    </button>
  </p>
  <p>Search icon on a styled link button:
    <a href="#" class="btn btn-info btn-lg">
      <span class="glyphicon glyphicon-search"></span> Search 
    </a>
  </p> 
  <p>Unicode:
    <span class="glyphicon">&#xe003;</span>
  </p> 
</div>

## Related:

 - [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
 - Beautiful Jekyll demo
