---
title: 借助Obsidian+QuickAdd实现快速写hugo博客
slug: obsidian-quickadd-hugo
description: 借助知识管理笔记软件Obsidian的插件QuickAdd，通过预设模板实现快速创建hugo文章。
categories:
  - life
tags:
  - Obsidian
  - hugo
draft: false
date: 2024-07-11 21:41:20
---

每次写博客时都要按照 Hugo 的格式增加如下头部信息，尽管我提前做了一个模板，每次复制模板，但多少还是有些不方便。

```
title: 
slug: 
description: 
categories: []
tags: []
draft: false
date: 
```

最近在研究一款功能极其强大的笔记管理工具—— [Obsidian](https://obsidian.md/)，很多人推荐用它做个人知识管理。Obsidian 的一些特点深深吸引了我：

1. **Markdown**：Obsidian 使用 Markdown 语法来编写和格式化笔记，这使得笔记内容简洁且易于编辑。
2. **本地存储**：所有笔记都保存在本地文件系统中，通常是纯文本文件（.md 格式），用户完全控制自己的数据，并且可以轻松备份和同步。
3. **双向链接**：Obsidian 提供强大的双向链接功能，通过在笔记之间创建互相引用的链接，构建一个复杂的知识网络。
4. **图谱视图**：通过图谱视图，用户可以可视化笔记之间的关系，帮助更好地理解和导航自己的知识库。
5. **插件系统**：Obsidian 支持丰富的插件，可以安装各种插件来扩展功能，例如快速输入、日历、任务管理、代码高亮等。
6. **自定义界面**：可以通过主题和 CSS 自定义 Obsidian 的界面，使其符合个人喜好。
7. **强大的搜索功能**：Obsidian 提供强大的搜索功能，能快速查找笔记内容和标签。
8. **社区支持**：Obsidian 拥有活跃的用户社区，有大量的用户交流经验、分享插件。

今天无意中看到了一个 QuickAdd 这个插件，可以按照自己的需求快速添加内容到笔记中，提高效率。看到有其他朋友用它了快速书写 Hugo 博客，也尝试了一把，极其舒适。

在操作前需要先制作一个 `新建文章` 的模板，使用 Obsidian 或者其他编辑器新建一个文件，命名为：新建博客.md（可以存放博客内容的文件夹，便于管理），并将如下内容填入：

```
---

title: {{NAME}}
slug: 
description: 
categories: []
tags: []
draft: false
date: {{DATE:YYYY-MM-DD HH:mm:ss}}

---
```

然后添加 QuickAdd 插件和具体配置，具体操作如下：

1. 在第三方插件中搜索：QuickAdd，安装并激活
2. 选择文章模板，选择存放内容的文件夹
3. 打开 Open the created file，并打开 Focus new pane（用来打开和定位到当前文件）

这些都配置好，就可以使用 QuickAdd 插件进行快速新建文章了，如下：

1. `command+p` 呼出命令看板
2. 输入 `qui` 就能看到 QuickAdd 插件了，回车确认
3. 看到刚创建的模板，再回车确认
4. 开始书写吧

