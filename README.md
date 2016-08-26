# rblog
Example blog with RStudio, RMarkdown and Jekyll.

## Prerequisits
<p>Install R language, RStudio, Git Bash and Jekyll(Optional if using Github pages)</p>
<p>Install the latest version of the knitr package: <code>install.packages("knitr")</code></p>
<p>Install other packages as per requirement, Like <code>install.packages("ggplot2");</code> for drawing graphs etc.</p>
<p>Make a theme in Jekyll or use ready-made ones available <a target="_blank" href="http://jekyllthemes.org/">here</a> for your blog</p>
<p>Make a new repository in <a href="https://github.com/">GitHub</a> with a default branch of gh-pages and upload that jekyll theme in it</p>
### Screenshot
![rblog screenshot](images/jekyll-themes.png)<br><br><br>
## Cloning jekyll blog in RStudio
<ul>
 <li>File, New project, Version control, Clone git</li>
 <li>Repository URL :<code>https://github.com/your repository</code></li>
 <li>Project directory name : your project directory name</li>
</ul>
### Screenshots
![rblog screenshot](images/new-project.png)<br><br>
![rblog screenshot](images/version-control.png)<br><br>
![rblog screenshot](images/git.png)<br><br>
![rblog screenshot](images/clone.png)<br><br>

## Publishing first post in your jekyll blog
<p>New post can be added by two methods<br><br>
<b>1. User interface</b><br>
<b>2. Command line</b><br>
</p>
### 1. User interface
<ul>
<li>First of all in RStudio goto <code>Tools -> Project Project Options -> Sweave -> Select knitr is default option -> Ok </code></li>
<li>You have to download <code>R Blog (Jekyll)</code> template from <a href="https://github.com/Tajtaj/r_blog/archive/master.zip">here</a></li>
<li>Place <code>r_blog</code> directory in <code>rmarkdown/rmarkdown/templates</code></li>
<li>After that goto <code>File-> New File -> RMarkdown -> From Template -> Select a template R Blog (Jekyll)</code></li>
<li>After that add RMarkdown code in the newly created file save it in <code>_posts</code> directory of your blog with the name  Y-M-D-title  e.g <code>2016-08-24-blogtitle</code> </li>
<li>As Jekyll supports markdown files, so you have to convert rmarkdown to markdown in RStudio by clicking Knit Html link</li>
<li>Now push only md files to github(if using gh-pages)</li>
<li>After that visit your blog and check the post</li>
</ul>
#### Screenshots
![rblog screenshot](images/default-option.png)<br><br>
![rblog screenshot](images/rmarkdown.png)<br><br>
![rblog screenshot](images/rblog-template.png)<br><br>
![rblog screenshot](images/default-screen.png)<br><br>
![rblog screenshot](images/output.png)<br><br><br><br><br>

### 2. Command line
<p>Making post from Command line requires some packages to install from RStudio console</p>
<ul>
<li><code>install.packages(c("knitr", "servr", "devtools"))</code></li>
<li><code>devtools::install_github("hadley/lubridate")</code></li>
<li><code>devtools::install_github("brendan-r/brocks")</code></li>
<li>After installation <code>brocks</code> package will appear in Packages of RStudio</li>
<li>By clicking <code>brocks</code> the user can see all the functions which <code>brocks</code> provides</li>
<li>After that write <code>library(brocks)</code> on RStudio console and hit enter</li>
<li>
  For making post from console <code>new_post(title = "new post", serve = TRUE, dir = "_source",
  subdir = TRUE, skeleton_file = ".skeleton_post")</code><br> 
  e.g <code>new_post(title = "This is second blog", serve = TRUE, dir ="F:/GitHub/rblog/_posts", subdir = FALSE)</code>
</li>
<li>Write your rmarkdown code</li>
<li>Click knit html link, it will produce md file, push that md file to github</li>
<li>Visit your blog the post will appear</li>
</ul><br><br>
#### Screenshots
![rblog screenshot](images/brocks.png)<br><br>
![rblog screenshot](images/brocks-functions.png)<br><br>




