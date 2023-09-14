基于主题 [NoCSS](https://github.com/g-hw/hugo-theme-nostyleplease) 二次修改

更新以下内容：

- 优化表格显示样式
- 优化代码高亮显示样式
- 优化cdn
- 添加Menus动态配置

 config配置：

```tomal
title = "demo"
theme = "lesscss"

[params]
  SEOTitle = "demo"
  Subtitle = "基于nocss二次调整的less css hugo博客主题"
  TOC = true

# 导航菜单
[[menu.main]]    
  identifier = "home"
  weight = 1   
  name = '🏠Home'
  url = "/"

[[menu.main]]
  identifier = "about"
  weight = 2
  name = "👨About"
  url = "/layout/about"

[[menu.main]]
  identifier = "search"
  weight = 3
  name = "🔍Search"
  url = "/layout/search"

# 代码高亮插件
[markup]
  [markup.highlight]
    anchorLineNos = false
    codeFences = true
    guessSyntax = true
    lineAnchors = ""
    lineNoStart =1
    lineNos = true
    lineNumbersInTable = true
    noClasses = true
    style = "dracula"
    tabWidth = 4

```

代码高亮插件参考文档：[Syntax highlighting | Hugo (gohugo.io)](https://gohugo.io/content-management/syntax-highlighting/)

代码高亮插件style在线预览：[Chroma Style Gallery (xyproto.github.io)](https://xyproto.github.io/splash/docs/all.html)

emoji地址：[ markdown-emoji ](https://gitcode.net/mirrors/zhouie/markdown-emoji?utm_source=csdn_github_accelerator)