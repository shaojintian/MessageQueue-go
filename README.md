# MessageQueue-go

⚡️一个基于主题-订阅模型的快速响应，高可用的消息队列

<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />

<p align="center">
  <a href="https://github.com/shaojintian/MessageQueue-go/">
    <img src="docs/images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Quick Response,High Availability</h3>
  <p align="center">
    An awesome MQ middleware to support your project!
    <br />
    <a href="https://github.com/shaojintian/MessageQueue-go"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/shaojintian/MessageQueue-go"> View Demo</a>
    ·
    <a href="https://github.com/shaojintian/MessageQueue-go/issues">Report Bug</a>
    ·
    <a href="https://github.com/shaojintian/MessageQueue-go/issues">Request Feature</a>
  </p>
  
</p>

架构图v0.0.1：蓝色代表线程分配，白色代表逻辑流
![architecture](docs/images/architecture.png)

Feature:(详细见src/docs/)
1. 主题发布-订阅模型
2. 全程无锁
3. Broker Cluster 的存储(元数据+消息)由开源的高性能Raft组[DragonBoat](https://github.com/shaojintian/dragonboat/blob/master/README.CHS.md)负责保证分布性一致性和容错性+[RocksDB](https://github.com/facebook/rocksdb/blob/master/INSTALL.md)负责持久化
4. 不采用刷盘做持久化也能达到直接刷盘的performance，集成更快



 本篇README.md面向开发者

## 目录

- [上手指南](#上手指南)
  - [开发前的配置要求](#开发前的配置要求)
  - [安装步骤](#安装步骤)
- [文件目录说明](#文件目录说明)
- [开发的架构](#开发的架构)
- [部署](#部署)
- [使用到的框架](#使用到的框架)
- [贡献者](#贡献者)
  - [如何参与开源项目](#如何参与开源项目)
- [版本控制](#版本控制)
- [作者](#作者)
- [鸣谢](#鸣谢)

### 上手指南





###### 开发前的配置要求

1. xxxxx x.x.x
2. xxxxx x.x.x

###### **安装步骤**

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo

```sh
git clone https://github.com/shaojintian/MessageQueue-go.git
```

### 文件目录说明

eg:

```
filetree 
├── ARCHITECTURE.md
├── LICENSE.txt
├── README.md
├── /account/
├── /bbs/
├── /docs/
│  ├── /rules/
│  │  ├── backend.txt
│  │  └── frontend.txt
├── manage.py
├── /oa/
├── /static/
├── /templates/
├── useless.md
└── /util/

```





### 开发的架构 

请阅读[ARCHITECTURE.md](https://github.com/shaojintian/MessageQueue-go/blob/master/ARCHITECTURE.md) 查阅为该项目的架构。

### 部署

暂无

### 使用到的框架

- [xxxxxxx](https://getbootstrap.com)
- [xxxxxxx](https://jquery.com)
- [xxxxxxx](https://laravel.com)

### 贡献者

请阅读**CONTRIBUTING.md** 查阅为该项目做出贡献的开发者。

#### 如何参与开源项目

贡献使开源社区成为一个学习、激励和创造的绝佳场所。你所作的任何贡献都是**非常感谢**的。

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



### 版本控制

该项目使用Git进行版本管理。您可以在repository参看当前可用版本。

### 作者

sjt@xxxx

[个人博客链接](https://www.shaojintian.cn)   

 *您也可以在贡献者名单中参看所有参与该项目的开发者。*

### 版权说明

该项目签署了MIT 授权许可，详情请参阅 [LICENSE.txt](https://github.com/shaojintian/MessageQueue-go/blob/master/LICENSE.txt)

### 鸣谢

- [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
- [Img Shields](https://shields.io)
- [Choose an Open Source License](https://choosealicense.com)
- [GitHub Pages](https://pages.github.com)
- [Animate.css](https://daneden.github.io/animate.css)
- [xxxxxxxxxxxxxx](https://connoratherton.com/loaders)

<!-- links -->

[your-project-path]: shaojintian/MessageQueue-go
[contributors-shield]: https://img.shields.io/github/contributors/shaojintian/MessageQueue-go.svg?style=flat-square
[contributors-url]: https://github.com/shaojintian/MessageQueue-go/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/shaojintian/MessageQueue-go.svg?style=flat-square
[forks-url]: https://github.com/shaojintian/MessageQueue-go/network/members
[stars-shield]: https://img.shields.io/github/stars/shaojintian/MessageQueue-go.svg?style=flat-square
[stars-url]: https://github.com/shaojintian/MessageQueue-go/stargazers
[issues-shield]: https://img.shields.io/github/issues/shaojintian/MessageQueue-go.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/shaojintian/MessageQueue-go.svg
[license-shield]: https://img.shields.io/github/license/shaojintian/MessageQueue-go.svg?style=flat-square
[license-url]: https://github.com/shaojintian/MessageQueue-go/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/shaojintian