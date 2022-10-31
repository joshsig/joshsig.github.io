# How to Host a Resume on GitHub Pages

How to create and host your resume on a website using a software stack.

1. [Instructions](#instructions)
   1. [Configuration]()
   2. [Installation]()
   3. [Operation]()
2. [Create your Resume using Markdown](#create-your-resume-using-markdown)
3. [Copyright]()
4. [Known-Bugs]()
5. [Troubleshooting]()
6. [Credits-and-Acknowledgements]()
7. [Contact]()
8. [Changelog]()

## Instructions
We will need to install a few things to achieve our goal of hosting our Resume on a website using Github Pages.

 - A mark-up language is very useful to learn and use. In Andrew Etter's Modern Technical Writing, he presses the importance of using a mark-up language to easily create XML that can then be shared with the world through Internet[^1]. I will be using Markdown out of all the possible mark-up languages because of it is the most widely used[^2]. 

 - Lets begin by installing a markdown and code editor. Personally I like to use [VS Code](https://code.visualstudio.com/download), you can use it to write Markdown and program your site as well. You can use any editor of your choice although. [Atom](https://atom.io/) is an editor specifically for Markdown. [Vim](https://vimhelp.org/) is an option for Markdown as well a code, not for the faint of heart.

![vscode](./)

 - You will also need some familiarity with Markdown to create our resume. Markdown is an easy-to-read, easy-to-write language for formatting plain text. I will be using GitHub Flavoured Markdown for this demonstration. If you are unfamiliar with Markdown reference [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) for basic syntax.
   
 - We will need to use the command line to install some dependencies for hosting our website. We are going to need Jekyll to host our website, and in order to get Jekyll we need Ruby (the language Jekyll is written in).
   - Install/Upgrade [Ruby](https://www.ruby-lang.org/en/documentation/installation/) 

   Run this command `ruby -v` to ensure ruby has been installed on your system.

   Follow set-up instructions for [Jekyll](https://jekyllrb.com/docs/installation/) and [Bundler](https://jekyllrb.com/docs/ruby-101/#gems)
   - Install Jekyll: `gem install jekyll bundler` 

 You will also need a [Github](https://github.com/) account as well as [Git Desktop](https://desktop.github.com/)! Your Github account will allow you to store all your code in a repository online for free! We can also use Git Desktop to connect the files on your computer to the repository very easily.

## Create your Resume using Markdown

Using Visual Studio Code, open a folder and create a new file. Name this file `resume.md`. Now that you have created a markdown file you have the ability to start writing your resume! Add your name, experience, education, etc. until you have a resume you want to share with the world! Reference [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) for any formatting needs.

## Running Locally
Compile and run your `Jekyll` website on your local network.
1. Ensure jekyll is installed: `jekyll -v`
2. Create your jekyll site: `jekyll new my-resume-site`
3. Navigate to the folder: `cd my-resume-site`
4. To host your website on your local network run, `bundle exec jekyll serve`

## Settings
You will want to customize the `_config.yml` to your own information.
### Site Settings
```
title: Your awesome title
email: your-email@example.com
description: your-description
twitter_username: your-twitter-username
github_username:  your-github
```

### Setup Repository
Navigate to [Github](https://github.com/) and create a repository. 

![Github Repository gif](https://media2.giphy.com/media/mgL99GKm27hZLZCbUC/giphy.gif?cid=790b7611df74b65c90b2a0f82e4dd3955b804307d3958091&rid=giphy.gif&ct=g)

[^1]: Andrew Etter - Modern Technical Writing, 33
[^2]: Andrew Etter - Modern Technical Writing, 39