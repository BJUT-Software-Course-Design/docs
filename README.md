# 项目文档

本文档为北京工业大学21级软件课设第8组的项目文档。

## 项目地址

Github团队地址: [https://github.com/BJUT-Software-Course-Design]

文档仓库地址: [https://github.com/BJUT-Software-Course-Design/docs]

前端仓库地址: [https://github.com/BJUT-Software-Course-Design/frontend]

后端仓库地址: [https://github.com/BJUT-Software-Course-Design/backend]

项目demo地址: [8.130.106.12]

## 文档编写方式

### 基础要求

本文档使用Markdown编写, 推荐使用Vscode编辑器, 搭配安装Markdown All in One插件, Markdown Preview Enhanced插件, 以及Markdownlint插件.

### 文档编写流程

首先加入Github组织, 而后fork本仓库, 在fork后的仓库中进行文档编写.

将仓库克隆到本地

```bash
git clone [你的仓库地址]
```

在本地编辑文档, 编写完成后, 提交到远程仓库

```bash
git add .
git commit -m "提交信息"
git push
```

注意: 在`git add .`之前, 请确保

1. 不要修改多余的文件, 以免提交到远程仓库(亦可在`git add`时指定需要添加的文件名).
2. (可选) 使用markdownlint插件检查文档格式是否符合规范.

提交信息请尽量简洁明了, 以便他人查看.

格式示例:

```bash
git commit -m "添加了项目开发计划章节"
```

在完成了一部分文档编写后, 可以提交pull request, 请求合并到主仓库. 具体操作方式请参考Github官方文档.

在代码合并到远程仓库后, 可以通过[Gitbook](https://noahs-organization-14.gitbook.io/docs/)查看文档效果(可能需要等待一段时间).

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

章节的格式示例如下, 以软件设计说明中的引言为例:

```markdown
# 3.1. 引言

## 3.1.1. 编写目的

本文档的读者人群为系统设计人员、系统开发人员、系统测试人员、系统维护人员、系统管理人员等。本文档的主要目的是对系统进行详细的设计说明，各个目标人群能够全面了解系统的设计思路、设计原则、设计方法、设计过程、设计结果等，以便于系统的实现、测试、维护和版本升级等。

## 3.1.2. 项目背景

......
```

注意在每个标题前加上序号, 序号后跟一个英文句点和一个空格.
