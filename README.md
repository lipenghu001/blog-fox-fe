![主页](http://cdn.friendlp.cn/1571331867191)

## 前言

此 blog 项目是基于 react 全家桶 + Ant Design 。

## 效果

效果图：

- pc 端

![首页](http://cdn.friendlp.cn/1571332246065)

- 移动端适配


完整效果请看：[http://www.friendlp.cn/](http://www.friendlp.cn/)

## 功能描述

### 已经实现功能

- [x] 登录
- [x] 注册
- [x] 文章列表
- [x] 标签分类
- [x] 个人介绍
- [x] 点赞与评论
- [x] 留言
- [x] 时间轴
- [x] 项目展示
- [x] 发文（支持 MarkDown 语法）
- [x] 文章详情展示（支持代码语法高亮）
- [x] 移动端适配
- [x] 网站波浪效果(请看 http://www.friendlp.cn/wave.html)
- [x] 第三方 github 授权登录
- [x] 文章归档
- [x] 文章详情的目录

### 待实现功能

- [ ] 无

## 前端技术

- react： ^16.8.4
- antd： ^3.15.0
- react-router:：^4.3.1
- webpack： 4.28.3
- axios：0.18.0
- redux: ^4.0.1
- highlight.js： ^9.15.6
- marked：^0.6.1

## 项目搭建

- 项目是按 antd 推荐的教程来搭建的：[antd 在 create-react-app 中使用](https://ant.design/docs/react/use-with-create-react-app-cn) , 实现了 按需加载组件代码和样式。

## 主要项目结构

```
- components
  - article 文章详情
  - articles 文章列表
  - comments 评论
  - loadEnd 加载完成
  - loading 加载中
  - login 登录
  - message 留言
  - nav 导航
  - project 项目
  - register 注册
  - slider 右边栏（博主 logo 、链接和标签等）
  - artchive 归档
  - timeLine 时间轴(历程)
- router 路由
- store redux 的状态管理
- utils 封装的常用的方法
- views 框架页面
```

## 注意点

- 关于 页面

对于 关于 的页面，其实是一篇文章来的，根据文章类型 type 来决定的，数据库里面 type 为 3
的文章，只能有一篇就是 博主介绍 ；达到了想什么时候修改内容都可以。

所以当 this.props.location.pathname === '/about' 时就是请求类型为 博主介绍 的文章。

```
type: 3, // 文章类型: 1：普通文章；2：是博主简历；3 ：是博主简介；
```

## Build Setup ( 建立安装 )

```
# install dependencies
npm install

# serve with hot reload at localhost: 3000
npm start 或者 yarn start

# build for production with minification
npm run build 或者 yarn run build
```

如果要看完整的效果，是要和后台项目 **[blog-fox-be](https://github.com/lipenghu001/blog-fox-be)** 一起运行才行的，不然接口请求会失败。

虽然引入了 mock 了，但是还没有时间做模拟数据，想看具体效果，请稳步到我的网站上查看 [http://www.friendlp.cn](http://www.friendlp.cn)

## 项目地址与文档教程


**项目地址：**

> [前台展示: https://github.com/lipenghu001/blog-fox-fe](https://github.com/lipenghu001/blog-fox-fe)

> [管理后台：https://github.com/lipenghu001/blog-fox-admin](https://github.com/lipenghu001/blog-fox-admin)

> [后端：https://github.com/lipenghu001/blog-fox-be](https://github.com/lipenghu001/blog-fox-be)

**本博客系统的系列文章：**

## 最后
