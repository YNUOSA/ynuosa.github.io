# Contribution Instructions

## Structure

|No.|Name|Description|
|---|----|-----------|
|01 |Home|主页门户入口，可以添加链接到开源中心其它服务|
|02 |Archives|自动生成归档，按时间，无需管理|
|03 |Tags|基于文章标签自动生成的「标签云」，无需管理|
|04 |Categories|文章分类<br>1. event 事件通知、预告、发布、总结<br>2.admin 站务信息，包括开源中心所有服务的维护信息<br>3.snippet 知识分享，分享知识、技术、开源项目|
|05 |About|关于页面，组织介绍|
|06 |Mirrors|链接到镜像站|
|07 |GitLab|链接到GitLab|
|08 |Wiki|链接到Wiki|

## Specification of Commit Message

### Usage

使用CI自动调用[Hexo](https://hexo.io/)生成静态页面并部署在主分支上，只需修改`/source`分支的源文件即可。

**注意配置 .gitignore, 建议 git add + 具体文件，以避免引入不必要的追踪项。**

### Specification

一行式标注，言简意赅描述更新内容，由<tag>和<message>组成:

```shell
git commit -m'(<tag>)<message>'
```
*中文允许，英文优先。**标点符号必须使用半角符号(西文符号)***

### TAGs

|TAG   |DESCRIPTION                                       |
|------|--------------------------------------------------|
|code  |更新代码，包含网站的程序、主题、配置文件等|
|fix   |仅指修复程序bug|
|doc   |修改文档，特指维护文档，不涉及网站内容|
|page  |修改了发布内容源文件。 `/source/_post` 下的普通文档和其他特殊页文档，对于普通页对应`<message>`应为`<category>/<title>`|
|revert|回滚到之前版本|
|host  |涉及托管的维护信息变更|

### Sample

```shell
git commit -m'(page)event/20170416-docker-offline-meeting '
```

## Design Guidelines

### Color Palette

- Primary Color: #FDD835
- Accent Color: #3F51B5
