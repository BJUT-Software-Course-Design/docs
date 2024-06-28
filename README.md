# 项目文档

本文档为北京工业大学21级软件课设第8组的项目文档。

## 文档编写方式

### 基础要求

本文档使用Markdown编写, 推荐使用Vscode编辑器, 搭配安装Markdown All in One插件, Markdown Preview Enhanced插件, 以及Markdownlint插件.

### 文档编写流程

将文档仓库克隆到本地

```bash
git clone git@github.com:BJUT-Software-Course-Design/docs.git
```

在本地编辑文档, 编写完成后, 提交到远程仓库

```bash
git add .
git commit -m "提交信息"
git push
```

注意: 在`git add .`之前, 请确保

1. 不要修改多余的文件, 以免提交到远程仓库.
2. (可选) 使用markdownlint插件检查文档格式是否符合规范.

提交信息请尽量简洁明了, 以便他人查看.

格式示例:

```bash
git commit -m "添加了项目开发计划章节"
```

在提交到远程仓库后, 可以通过[Gitbook](https://noahs-organization-14.gitbook.io/docs/2-xu-qiu-gui-ge-shuo-ming)查看文档效果(可能需要等待一段时间).

### 章节划分

本文档分为以下几个部分:

* 项目开发计划
* 需求规格说明
* 软件设计说明
* 项目开发记录
* 测试记录
* 用户操作手册

每个部分根据模板, 分为若干个章节, 在编写文档时, 每个章节**在对应文件夹中建立一个新的Markdown文件**, 起名为`章节名.md`, 并在SUMMARY.md中添加链接(相对路径).

示例:

```markdown
* 1. 项目开发计划
  * [1.1. 引言](项目开发计划/引言.md)
  * [1.2. 项目概述](项目开发计划/项目概述.md)
```

### 图片引用

当需要引用图片时, 请将图片放置在`images`文件夹中, 并在Markdown文件中使用相对路径引用.

示例:

```markdown
![图片描述](images/图片名.png)
```

### 章节格式

每个章节的格式如下:

```markdown
# 章节名

## 章节内小节名

### 章节内小节内小节名
```
