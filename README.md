# rblog
Example blog with RStudio, RMarkdown and Jekyll.

## Prerequisits
<p>Install R language, RStudio, Git Bash and Jekyll</p>
<p>Install the latest version of the knitr package: <code>install.packages("knitr")</code></p>
<p>Install other packages as per requirement, Like <code>install.packages("ggplot2");</code> for drawing graphs etc.</p>
<p>Make a theme in Jekyll or use <a target="_blank" href="http://jekyllthemes.org/">ready-made ones</a> available for blog</p>
<p>Make a new repository with a default branch of gh-pages and upload that jekyll theme in it</p>

## Cloning jekyll blog in RStudio
<ul>
 <li>File, New project, Version control, Clone git</li>
 <li>Repository URL :<code>https://github.com/your repository</code></li>
 <li>Project directory name : your project directory name</li>
</ul>
## Publishing first post in jekyll blog
<p>
<ul>
<li> Make Rmd file in RStudio convert it to md file</li>
<li> Put the md file in _posts folder of jekyll blog</li> 
<li>File name should be like Y-M-D-title.md  e.g <code>2016-08-24-blogtitle.md</code></li>
<li>Add required Front Matter to the newly created md file<br>
<code>
<pre>
---
layout: post
title: blog title
---
</pre>
</code>
</li>
<li>Push changes to github</li>
</ul>
</p>
## Ready
<p>Goto settings of repository and visit the url<br>
e.g <a href="https://project-spinoza.github.io/rblog/">Visit Blog</a>
</p>
## Example 
![rblog screenshot](screenshot.png)

