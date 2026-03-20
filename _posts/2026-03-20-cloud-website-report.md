# 云计算网站部署实验报告

## 一、实验目的
本实验旨在通过实践操作，掌握基于云计算环境的网站部署技能。
具体包括：构建环境并实现个人博客/网站的搭建，撰写实验报告，并将这份报告作为一篇博文发布在自己的博客 / 网站上。

## 二、实验环境
- 硬件环境： 
联网的计算机一台

- 软件环境：
操作系统：Windows 11
云计算平台：GitHub Pages
工具：VS Code、Git

## 三、实验步骤
1. 基于开源模板搭建云计算博客框架
选用GitHub开源仓库chirpy-starter（仓库地址：https://github.com/cotes2020/chirpy-starter）作为博客搭建的核心模板。该仓库是基于Jekyll构建的轻量化静态博客模板，专为GitHub Pages优化，具备响应式布局、文章分类、标签检索、夜间模式等完整的博客功能，无需编写复杂的前端代码，仅需通过简单的配置和内容编写即可完成个人网站的搭建。

![chirpy-starter](images/1.png)

GitHub Pages是GitHub提供的免费静态网站托管服务（云计算PaaS层服务），chirpy-starter模板预先封装了Jekyll静态站点生成规则，用户通过“模板复用”（Use this template → Create a new repository）创建专属仓库后，GitHub会自动识别模板中的配置文件和内容文件，将Markdown格式的博客文章编译为HTML/CSS/JS静态资源，并部署到GitHub的云端服务器上，最终通过“用户名.github.io”域名对外提供访问服务。

![命名仓库](images/2.png)

套用模板：

![套用模板](images/3.png)

2. 本地环境操作与云端发布
打开目标文件夹，打开Git终端执行克隆命令git clone https://github.com/lay1260/lay1260.github.io.git，将云端的博客仓库完整复制到本地。

![克隆](images/4.png)

克隆完成后本地生成“lay1260.github.io”文件夹（即博客仓库根目录），该文件夹包含 _posts（博客文章存储目录）、_config.yml（博客配置文件）、README.md（说明文档）等核心文件。

![本地仓库](images/5.png)

在本地博客仓库的_posts子文件夹中，新建Markdown格式文件，命名为 2026-03-20-cloud-website-deployment-report.md，以Markdown语法编写实验报告。

![撰写报告文件](images/6.png)

在Git Bash终端将本地编写的实验报告、图片等所有修改文件加入暂存区，为本次修改添加版本记录，再将本地暂存的内容推送到 GitHub 云端仓库。

![推送](images/7.png)

![成功](images/8.png)

GitHub Pages自动完成静态资源编译和部署，通过浏览器访问 https://lay1260.github.io，可查看到实验报告已作为博客文章发布在自建网站中，验证发布成功。

![Home页面](images/9.png)

![博客页面](images/10.png)

## 四、结论分析与体会
本次实验借助GitHub Pages云计算平台与chirpy-starter开源模板，成功完成了个人博客的搭建，并将云计算网站部署实验报告以博文形式发布至自建博客。实验结果验证了GitHub Pages作为轻量级云计算PaaS层服务的实用性，其依托Git版本控制实现本地与云端的内容同步，结合Jekyll静态站点生成技术，能快速将Markdown格式的文本编译为可公网访问的静态网页，无需搭建本地服务器、无需投入服务器运维成本，即可实现个人网站的快速部署与发布，是云计算技术在轻量级网站搭建场景中的典型应用。