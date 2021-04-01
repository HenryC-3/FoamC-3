### 前言

[FoamC-3](https://github.com/HenryC-3/FoamC-3) 基于:

- [foambubble/foam-template: Foam workpace template](https://github.com/foambubble/foam-template)
- [spencerwooo/foam-wiki: Foam as second brain. Powered by VuePress.](https://github.com/spencerwooo/foam-wiki)

在线地址: [Henry's Wiki](https://henryc-3.github.io/FoamC-3/)

### 项目目录

```text
├── .vscode
├── .vuepress
├── attachments
├── examples
├── inbox.md
├── index.md
├── README.md
├── theme
```

- .vscode: vscode 工作区配置文件
- .vuepress: vuepress 配置文件
- thmeme: vuepress 主题配置
- attachments: 附件
- examples: 示例
- inbox.md: 收集箱
- index.md: 根文件, 也是部署 `GitPage` 的首页

### 插件集合

- foam: 提供 wikilink, note graph, backlink, tag 功能
- markdown Preview mermaid: mermaid markdown 预览
- Mermaid Markdown Syntax Highlighting: mermaid 语法高亮
- vscode-drawio: 在 vscode 中使用 drawio, 相较于使用 drawio 桌面端, 使用该插件能够从 vscode 中无缝跳转至 drawio
- vscode-drawio-mermaid-plugin: 支持在 drawio 中绘制 mermaid
- TODO tree: 寻找文件的所有 TODO 并集中显示, 用于完成简单的 GTD 功能

### 用法

- 在项目根目录下新建 `docs` 文件夹, `.gitignore` 中添加 `./docs/node_modules`
- 拉取仓库, 删除 `docs` 中 `.gitignore`
- 使用 vscode 打开 `docs` 工作区, 安装推荐插件
- 在 `index.md` 中组织笔记结构, 使用 foam `show graph` 或者 `orphan view` 查看零散笔记

### Q&A

1. 为什么删除 `docs` 文件夹下的 `gitignore` ?
   - 于我而言, `docs` 中的内容是笔记, 相当于增强版 `git message` 因此与代码同步进行版本管理
