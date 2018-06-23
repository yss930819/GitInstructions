# Git使用教程

- <font color="red">为什么要编写这个教程？</font>
> 命令行操作Git对于任何人来说都是一种不愉快的体验，更多的人对于命令行是畏之如虎。
>
> 因此当你想向同事推广使用Git时，你会发现这是一件很艰难的事。他们反应都是：*什么？这个要用命令行？我拒绝！！！*
>
> 因此本教程诞生了，基于windows 和 一个较为易用GUI软件说明Git 的使用方法，从而可以快速将Git用于工作中，Git就是一个工具会用就行。

- <font color="red">为什么要使用git？</font>（下面摘自[廖雪峰的网站](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001373962845513aefd77a99f4145f0a2c7a7ca057e7570000)：）
> 如果你用Microsoft Word写过长篇大论，那你一定有这样的经历：
>
> 想删除一个段落，又怕将来想恢复找不回来怎么办？有办法，先把当前文件“另存为……”一个新的Word文件，再接着改，改到一定程度，再“另存为……”一个新文件，这样一直改下去，最后你的Word文档变成了这样：
>
> ![lots-of-docs](./img/0.jpg)
>
> 过了一周，你想找回被删除的文字，但是已经记不清删除前保存在哪个文件里了，只好一个一个文件去找，真麻烦。
>
> 看着一堆乱七八糟的文件，想保留最新的一个，然后把其他的删掉，又怕哪天会用上，还不敢删，真郁闷。
>
> 更要命的是，有些部分需要你的财务同事帮助填写，于是你把文件Copy到U盘里给她（也可能通过Email发送一份给她），然后，你继续修改Word文件。一天后，同事再把Word文件传给你，此时，你必须想想，发给她之后到你收到她的文件期间，你作了哪些改动，得把你的改动和她的部分合并，真困难。
>
> 于是你想，如果有一个软件，不但能自动帮我记录每次文件的改动，还可以让同事协作编辑，这样就不用自己管理一堆类似的文件了，也不需要把文件传来传去。如果想查看某次改动，只需要在软件里瞄一眼就可以，岂不是很方便？
>
> 这个软件用起来就应该像这个样子，能记录每次文件的改动：
>
| 版本 | 文件名 | 用户 | 说明 | 日期 |
| ---- | ------ | ---- | ---- | ---- |
| 1 | service.doc | 张三 | 删除了软件服务条款5 | 7/12 10:38 |
| 2 | service.doc | 张三 | 增加了License人数限制 | 7/12 18:09 |
| 3 | service.doc | 李四 | 财务部门调整了合同金额 | 7/13 9:51 |
| 4 | service.doc | 张三 | 延长了免费升级周期 | 7/14 15:17 |
> 这样，你就结束了手动管理多个“版本”的史前时代，进入到版本控制的20世纪。

## 软件下载地址

1. Git Windows版本 : [官方](https://git-scm.com/download/win)   [淘宝镜像](https://npm.taobao.org/mirrors/git-for-windows/)
1. TortoiseGit : [官方](https://tortoisegit.org/download/)
1. Gitea : [官方](https://dl.gitea.io/gitea/)  [Github](https://github.com/go-gitea/gitea/releases)

------
其他 gui软件
1. SmartGit ： [官方](https://www.syntevo.com/smartgit/download/) *经测试该软件更为好用，但是软件全为英文*
1. SourceTree ： [官方](https://www.sourcetreeapp.com/)
1. VsCode : [官方](https://code.visualstudio.com/)  *安装GitLens插件效果更好*

## 快速上手
这里包含了一组让Git的使用样例，通过样例让您快速了解Git简单的使用方法，并将其运用到工作中。

- [一台新电脑的开始](./快速上手/一台新电脑的开始/)  
    本部分教程将教你如何在一台全新的电脑上安装git和使用相关的GUI工具（我们以TortoiseGit为教程对象）。
 
- [本地简单使用](./快速上手/本地简单使用/)  
    本部分介绍了，Git在不与远端协同使用的场景。主要为新建、提交和版本浏览。
    
- [Git服务器搭建](./快速上手/Git服务器搭建/)  
    本部分介绍了，Gitea服务器的简单搭建了配置方法，可以快速上手进行GIT使用。

- [Git协作之旅](./快速上手/Git协作之旅/)  
    本部分介绍了，使用Gitea的简单方法，主要为项目的克隆、拉取和推送。
     
- [疑难解答](./快速上手/疑难解答/)  
    本部分总结了新手可能遇到的各种问题，当遇到问题时就及时看过来吧~~

## 高手进阶

- [Gitea服务的进阶配置](./高手进阶/Gitea服务的进阶配置/)  
    本部分介绍了Gitea服务器的进阶配置方法，包括使用离线模式，提高上传附件限制。

- [Gitea的进阶使用](./高手进阶/Gitea的进阶使用/)  
    本部分介绍了Gitea的进阶使用方法，包括使用工单系统，建立组织，在组织中建立权限不同的团队等。

- [SmartGit的使用说明](./高手进阶/SmartGit的使用说明/)  
    可能，现在你已经有了数十个仓库需要进行管理，再使用TortoiseGit你会觉得非常不方便，特别是在不同项目之间的切换。
    那么你现在需要使用一个'*进阶*'的Git GUI软件了--- SmartGit。本部分将详细介绍SmartGIT的使用方法！你将发现你会进入一个不一样的世界。