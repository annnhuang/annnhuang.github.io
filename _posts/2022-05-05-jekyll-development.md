---
layout: post
title:  "Create a website using Jekyll & Github under 5 minutes"
subtitle:  "Great fun, very useful, and completely free"
date:   2022-05-05
tags: [general]
---

Here are 10 steps to create a website using Jekyll and host it using Github Pages.

## 1. Download and install the necessary dependencies:

(a) [Ruby](https://jekyllrb.com/docs/ruby-101/) (Jekyll is written in Ruby)
  - Windows: Install RubyInstaller. Choose a version that includes DevKit.
  - Mac: Ruby comes pre-installed on macOS, but you can update it via Homebrew:

  ```
  > brew install ruby
  ```

(b) [Bundler](https://jekyllrb.com/tutorials/using-jekyll-with-bundler/) (a development tool that combines JavaScript code files into a single one that is production-ready loadable in the browser)

```
> gem install bundler
```

(c) Jekyll (The static site generator)

Install Jekyll using Bundler:

```
> gem install jekyll
```
(d) [Git](https://git-scm.com/downloads) (for version control and pushing to GitHub)

## 2. Choose a [theme](https://jekyllrb.com/docs/themes/)

## 3. Download the theme

- Find the theme’s GitHub repository (e.g., Minimal Mistakes), click "<> Code", and download the ZIP file.

## 4. Unzip or extract the files and place them in a directory where you want to manage your Jekyll site

## 5. Open the files using any code editor
-  For example, Visual Studio Code is a popular choice

## 6. Run Jekyll locally

- Navigate to your project folder, and type in the terminal:

```
> bundle exec jekyll serve
```

- Copy the localhost URL (e.g., http://127.0.0.1:4000) and paste it into your browser to preview your site.

## 7. Link Jekyll to a Github repository

(a) Create a repository on Github
- Go to GitHub and sign in.
- Click on "New Repository".
- If you want your site to be hosted as "https://your-github-account-name.github.io", simply name the repository "your-github-account-name.github.io"

(b) Initialize a Git repository in your local project
- Open the terminal inside your Jekyll project folder and run:

```
> git init
```

- This initializes Git in your project.

(c) Connect your local project to GitHub

```
> git remote add origin https://github.com/your-github-account-name/your-repo-name.git
```

(d) Add and commit the Files

```
> git add . 
> git commit -m "Initial commit - Jekyll site"
```

(e) Push the project to GitHub (it’s either the main branch or the master branch)

```
> git branch -M main
> git push -u origin main
```

## 8. Enable GitHub Pages
- Go to your GitHub repository.
- Click Settings > Pages.
- Under "Branch," select main (or gh-pages if you set it up that way).
- Click Save.
- After a few minutes, your website will be live at https://your-github-account-name.github.io.

## 9. Final notes

(a) If your theme has extra dependencies, install them with:

```
> bundle install
```

(b) To update your site, modify the files, commit changes, and push them to GitHub:

```
> git add .
> git commit -m "Update site"
> git push origin main
```

## 10. Happy blogging!

## 11. Learn more about working with the folder structures [here](https://www.youtube.com/watch?v=T1itpPvFWHI&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&ab_channel=GiraffeAcademy)