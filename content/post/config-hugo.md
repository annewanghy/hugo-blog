---
title: "Config Hugo"
date: 2018-03-04T17:07:36+08:00
draft: true
---

## Install hugo on mac-os use brew

```
1.  brew install hugo
2.  brew upgrade hugo
3.  hugo version
    Hugo Static Site Generator v0.37 darwin/amd64 BuildDate
4.  git clone https://github.com/olOwOlo/hugo-theme-even themes/even
5.  在主题的 exampleSite 目录下有一个 config.toml 文件，将这个 config.toml 文件复制到你的站点目录下，根据自己的需求更改即可。
6.  hugo new post/first.md
7.  hugo server --theme="even" --buildDrafts
8.  git init
9.  echo "themes/" >> .gitignore
10. echo "public" >> .gitignore
11. git init
12. git add remote origin https://github.com/annewanghy/hugo-blog.git
12. git add .
13. git push
```

### Use github pages

```
1. hugo --theme=even --buildDrafts --baseUrl="https://annewanghy.github.io/"
2. cd public
3. git init
4. git add remote origin https://github.com/annewanghy/annewanghy.github.io.git
5. git add .
6. git push
```

### Add shell file to auto deploy

```shell
hugo --theme=even --buildDrafts --baseUrl="https://annewanghy.github.io/"
cd public
git add .
git commit -m "Update blog"
git push
```
