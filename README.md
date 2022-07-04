- [Hango Blog介绍](#hango-blog介绍)
  - [本地调试GIthub Pages](#本地调试github-pages)
    - [安装](#安装)
    - [本地运行](#本地运行)
  - [添加Blog](#添加blog)



# Hango Blog介绍


[Hango Blog](https://github.com/hango-io/hango-io.github.io)基于[Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll)改造而来，旨在提供Hango项目的官方教程和相关博客。


## 本地调试GIthub Pages

### 安装

- 根据[Jekyll Installation](https://jekyllrb.com/docs/installation/)，确保[Requirements](https://jekyllrb.com/docs/installation/#requirements)全部满足
- 根据[Guides](https://jekyllrb.com/docs/installation/#guides)，根据OS，安装依赖



### 本地运行

ubuntu系统为例

- 进入本地 `hango-io.github.io`项目文件夹
- `source ~/.bashrc`
- 执行`bundle exec jekyll serve`，可在本地4000端口访问界面。

详情参见[使用 Jekyll 在本地测试 GitHub Pages 站点](https://docs.github.com/cn/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)





## 添加Blog

1. 进入`_posts/[category]`文件夹下，添加posts文件，文件名称必须是"YYYY-MM-DD-Title.md"的格式

2. 添加文件头，如下

   ```yaml
   ---
   layout: post	# 固定内容，表明文件形式是博客文章
   title: 高性能云原生网关Hango1.0架构	# 自定义，标题
   subtitle: 基于Istio以及Envoy构建的高性能云原生API网关 Hango # 自定义，副标题
   cover-img: /assets/img/path.jpg	# 自定义，博客页面置顶的图片
   thumbnail-img: /assets/img/thumb.png	# 自定义，网站主页处该博客的配图
   share-img: /assets/img/path.jpg	# 自定义，分享该博客的链接封面图
   tags: [overview]	# 自定义，博客的提示标签，可以多个，逗号分割
   categories: overview	# 表明博客所属分类，在[overview, plugin, release-notes, others]中选择一个
   ---
   
   目录]
   
   [正文]
   ```

3. 文章创建完成后，本地刷新服务器即可查看，文章地址一般是`https://localhost:4000/[category]/[title]`



