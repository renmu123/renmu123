---
title: 程序员必备的Obsidian插件
date: 2021-05-08 11:40:41
tags:
---

我介绍一个程序员使用 Obsidian 来进行写作所必要的插件以及使用方法。
其中在我进行写作的时候发现有几个流程不是很顺畅，也自己尝试创建了项目，以及对一些项目进行了 PR。

<!-- more -->

# Prettier Format

## 介绍

这是一个利用 `prettier` 来将 `markdown` 进行格式化的工具，同时也支持对 `html` 和 `js` 代码块进行格式化。

## 安装

在社区插件中搜索 `prettier format` 点击安装。
或者使用 github 手动安装：https://github.com/hipstersmoothie/obsidian-plugin-prettier

## 使用

安装完成后，输入 `Ctrl+P`，在弹出框中输入 `format the entire note`，进行文档的格式化。
如果你也认为每次这样操作是比较麻烦的，你可以在快捷键设置中为这个命令设置快捷键，或者直接在插件设置选项设置 `format on save` 选项为 `true`，这样在文件保存时会触发自动格式化。

# Editor Syntax Highlight

## 介绍

使你的代码在编辑模式下也可以直接进行语法高亮

## 安装

在社区插件中搜索 `Editor Syntax Highlight` 点击安装。
或者使用 github 手动安装：https://github.com/deathau/cm-editor-syntax-highlight-obsidian

## 使用

没什么好说的，安装即用，很香。

# Obsidian Tabs

## 介绍

这允许你能打开多个页面并直接在编辑栏上方进行切换。

## 安装

在社区插件中搜索 `obsidian tabs` 点击安装。
或者使用 github 手动安装：https://github.com/gitobsidiantutorial/obsidian-tabs

## 使用

你可以在笔记栏使用 `Ctrl+左键` 来在 `tab` 打开。

更多细节上的设置请看该插件的设置项。简单翻译了一下，还有几个的选项的用处自己探索吧。

| 设置项 | 含义 |
| Enable Obsidian Tbas | 是否启用插件 |
| Two Row Tab Overview | tab 量多了会智能变成两行 |
| Tab Height | tab 高度，默认 29 |
| proper Horizontai Splits | |
| Show Tab Buttons | 允许插件拖动布局 |
| Full Sized Title Text | |
| Full Tab Spacing | |
| Remove Tab Numbers | 移除 Tab 上的数字 |
| Remove Tab Underline | 移除下一个页面的下划线 |

# Image auto upload Plugin

# Code block from selection

## 介绍

利用快捷键快速插入代码块

## 安装

## 使用

作为程序员写笔记的时候要经常插入代码块，但 Obsidian 初始的插入方式要足足按七下键盘，还不包括输入语言，实在是太痛苦了。推荐程序员必备！

安装完成后，在插件的配置页配置需要快速生成的语言（如 js,python,html）目前最多只支持三个。
之后你可以采用 `Ctrl+P` 呼出命令面板来进行插入或者像我一样直接在快捷键中绑定该命令（推荐），妈妈再也不用担心我快速输入代码块了。

# paste URL into selection

## 介绍

该插件可以快速插入网址

## 安装

在社区插件中搜索 `paste URL into selection` 点击安装。
或者使用 github 手动安装：https://github.com/denolehov/obsidian-url-into-selection

## 使用

当你的剪切板中有网址时，选择文字，点击复制，就会自动生成符合 markdown 的超链接，再也不用手动一个一个输入了。插件设置中有直接自动选中插入的选项，有兴趣的可以尝试一下。

# Hot Reload

## 介绍

这是一个给开发者使用的插件，用于修改代码后热加载插件，使你从手动工作中解脱出来。

## 安装

仅支持 github 手动安装：https://github.com/pjeby/hot-reload
将代码下载解压后扔到 `.obsidian/plugins/` 文件夹，然后在第三方插件中进行启用

## 使用

该插件会对你的插件文件夹进行监视（仅当该文件夹中有 `.git` 或者 `.hotreload` 时），如果有变动，便会利用 Obsidian API 来对该插件进行禁用以及启用，以达到手动禁用启用的效果，除此之外这个插件不会做任何额外的工作。
