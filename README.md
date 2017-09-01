# Starting from generating a mkdocs project

## Install mkdocs cli
```
sudo pip install mkdocs
```

## Create a new mkdocs project
```
mkdocs new testmkdocs
```

## Edit mkdocs.yml for adding chapters
cat mkdocs.yml (for example)
```
site_name: The Field Guide to Open Source in the Newsroom
pages:
    - Home: index.md
    - Chapter 1 - Choosing Open Source, Getting Buy-In: Chapter01-Choosing-Open-Source.md
    - Chapter 2 - Starting a New Project: Chapter02-Starting-New-Project.md
    - Chapter 3 - Opening Up An Existing Project: Chapter03-Existing-Projects.md
    - Chapter 4 - Code & Getting To The First Release: Chapter04-Code-First-Release.md
    - Chapter 5 - Documentation: Chapter05-Documentation.md
    - Chapter 6 - Working With Community: Chapter06-Community.md
    - Chapter 7 - Managing Releases: Chapter07-Releases.md
    - Chapter 8 - Handoffs & Sunsets: Chapter08-Handoffs-Sunsets.md
    - Contribute to this guide: contributing.md
    - Help: help.md
theme: readthedocs
```

## Creating empty markdown files for each chapters, for example
``` 
cd testmkdocs/docs
touch Chapter02-Starting-New-Project.md
touch Chapter03-Existing-Projects.md
touch Chapter04-Code-First-Release.md
touch Chapter05-Documentation.md
touch Chapter07-Releases.md
touch Chapter08-Handoffs-Sunsets.md
touch contributing.md
touch help.md
touch Chapter06-Community.md
```

## Start mkdocs server
```
mkdocs serve
```

## Git your document
```
cd testmkdocs
git init
git add -A
git commit -m'init'
```

## Create a git repo on github, if you want to deploy to github
then
```
git remote add origin git@github.com:mingderwang/testmkdocs.git
```
for example

## Deploy your mkdocs to github
```
mkdocs gh-deploy
```
