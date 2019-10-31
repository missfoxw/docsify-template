下载的模板结构如下：
```yml
docsify-template
├─docs docsify文档目录
│  ├─src 文件夹-主体内容
│  │  ├─1 文件夹-关于本文档
│  │  │  └─README.md markdown文件-关于本文档
│  │  │
│  │  ├─2 文件夹-快速开始
│  │  │  └─README.md markdown文件-快速开始
│  │  │
│  │  └─3 文件夹-模板说明
│  │     └─README.md markdown文件-模板说明
│  │
│  ├─static 文件夹-引用脚本相关
│  │  ├─docsify 文件夹
│  │  │  ├─lib 文件夹-docsify依赖 此处不展开
│  │  │  └─themes 文件夹-包含主题css 此处不展开
│  │  │
│  │  ├─docsify-pagination 文件夹-分页依赖 此处不展开
│  │  │
│  │  ├─mermaid 文件夹-支持mermaid的依赖 此处不展开
│  │  │
│  │  └─prismjs 文件夹-支持语法高亮依赖 此处不展开
│  │
│  ├─_coverpage.md markdown文件-封面
│  ├─_navbar.md markdown文件-导航
│  ├─_sidebar.md markdown文件-菜单
│  ├─.nojekyll 空文件-用于阻止 GitHub Pages 会忽略掉下划线开头的文件
│  ├─index.html 入口文件(配置都在这里)
│  ├─my404.md markdown文件-404
│  └─README.md markdown文件-文档说明，会作为主页渲染
│  
└─README.md 整体说明
```

src文件夹内可以归类需要写的各章节内容，也可以在docs下新建其他文件夹或其他markdown文件作为章节内容。