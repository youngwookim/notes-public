# Atom + MPE plugin + MacTex + pandoc

Markdown for reports at work???

## Install & configure MacTex
```
brew cask install mactex

sudo tlmgr repository add http://ftp.ktug.org/KTUG/texlive/tlnet ktug
sudo tlmgr pinning add ktug "*"
sudo tlmgr install nanumttf hcr-lvt
sudo tlmgr update --all --self
```

## Install pandoc
```
brew install pandoc
```

## Install Atom Editor & MPE plugin
- Atom Editor
```
brew cask install atom
```
- Install MPE plugin


## Exmaples

example.md:
```

---
title: "Doc Title"
author: John Doe
date: March 22, 2005
output:
  pdf_document:
    latex_engine: xelatex
    toc: true
    toc_depth: 3
papersize: A4
fontsize: 11pt
mainfont: NanumGothic
---

# Title 1

1. this is ...

Answer to original question...

\newpage

# Title 2
## Sub-title 1

Tables

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

foot note:

Content [^1]

[^1]: Hi! This is a footnote
```
