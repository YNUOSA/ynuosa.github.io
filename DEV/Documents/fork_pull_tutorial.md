# [YNUOSA主页](https://ynuosa.org) FORK&PULL教程

## 常用链接

- 项目地址 https://github.com/YNUOSA/ynuosa.github.io
- 源码地址(`/source`分支) https://github.com/YNUOSA/ynuosa.github.io/tree/source
- 公共文档 https://github.com/YNUOSA/ynuosa.github.io/tree/source/DEV
- TravisCI项目 https://travis-ci.org/YNUOSA/ynuosa.github.io

## 基础发布步骤

以我的ID为例([@posoo](https://github.com/posoo)),具体请替换为自己的ID

### 1. fork该项目

将[该项目](https://github.com/YNUOSA/ynuosa.github.io)fork到自己ID的名下

![Screen_Shot_2017-05-04_at_3_31_25_PM.png](https://ooo.0o0.ooo/2017/05/04/590ae6f0f1724.png)

clone该项目并进入项目目录

```shell
git clone git@github.com:posoo/ynuosa.github.io.git
cd ynuosa.github.io
```

### 2. 切换到`/source`分支

```shell
git checkout source
```
![Screen Shot 2017-05-04 at 3.38.22 PM.png](https://ooo.0o0.ooo/2017/05/04/590ae6ef7e10b.png)


### 3. 进入文章源目录

```shell
cd source/_posts
```

### 4. 创建并编辑Markdown格式文档

**格式参见[该目录](https://github.com/posoo/ynuosa.github.io/tree/source/DEV/Templates)下的相关模版**

![Screen Shot 2017-05-04 at 3.58.10 PM.png](https://ooo.0o0.ooo/2017/05/04/590adfa66d161.png)

### 5. git add&commit&push

**commit message格式参见[此文档](https://github.com/posoo/ynuosa.github.io/blob/source/DEV/Documents/contribution_instructions.md)**

![Screen Shot 2017-05-04 at 4.00.05 PM.png](https://ooo.0o0.ooo/2017/05/04/590adfa730bc6.png)

### 6. pull request

在[YNUOSA/ynuosa.github.io](https://github.com/YNUOSA/ynuosa.github.io/pulls)项目中新建一个`Pull Request`

![Screen_Shot_2017-05-04_at_4_07_14_PM.png](https://ooo.0o0.ooo/2017/05/04/590ae476046d8.png)

进行对应分支的比较

![Screen_Shot_2017-05-04_at_4_11_20_PM.png](https://ooo.0o0.ooo/2017/05/04/590ae4785785c.png)

创建评论

![Screen Shot 2017-05-04 at 4.18.18 PM.png](https://ooo.0o0.ooo/2017/05/04/590ae4776f303.png)

`Pull Request` 创建成功，进入等待队列 (TravisCI会自动检测冲突)

![Screen Shot 2017-05-04 at 4.19.07 PM.png](https://ooo.0o0.ooo/2017/05/04/590ae47830b54.png)

### 7. 等！等等等！等！

通过项目管理员审核并merge后，会自动通过TravisCI生成静态页面部署在`／master`分支。


