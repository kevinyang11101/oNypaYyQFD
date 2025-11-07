# 在线BLOG网 - Java毕业设计分享

## 前言

此项目为基于Java语言的在线BLOG网，是计算机毕业生的实战项目。本项目不仅包含了完整的源码，还附有详细的文档报告和代码讲解，旨在帮助学习者深入理解并掌握Java Web开发技术。

## 内容介绍

本项目是一个功能齐全的在线BLOG网站，用户可以发布文章、评论和交流。系统后端采用Java语言结合Spring Boot框架进行开发，前端则运用了JS、Vue和CSS3等技术。通过此项目，可以学习到前后端的交互逻辑、数据库设计以及用户界面的构建。

## 技术介绍

- **语言：** Java
- **使用框架：** Spring Boot
- **前端技术：** JS、Vue、CSS3
- **开发工具：** IDEA/Eclipse
- **数据库：** MySQL 5.7/8.0
- **数据库管理工具：** phpstudy/Navicat
- **JDK版本：** jdk1.8
- **Maven：** apache-maven 3.8.1-bin
- **前端环境：** Node.Js 12\14\16

## 核心代码

以下是项目中处理文章发布的部分核心代码：

```java
// ArticleController.java

@PostMapping("/publish")
public ResponseEntity<?> publishArticle(@RequestBody Article article, Principal principal) {
    if (principal == null) {
        return new ResponseEntity<>(HttpStatus.UNAUTHORIZED);
    }
    String username = principal.getName();
    User user = userService.findByUsername(username);
    article.setUser(user);
    Article savedArticle = articleService.save(article);
    return new ResponseEntity<>(savedArticle, HttpStatus.CREATED);
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img13.360buyimg.com/ddimg/jfs/t1/319364/3/26034/139207/689f009cF7e8fbddb/06bddd2360922936.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/309756/22/26473/102924/689f0078F349a6c1f/4eb27adc98934712.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/316460/5/26098/101757/689f0079Fcba6ce5a/e8711d5694523192.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/320806/7/25918/16693/689f007aF4e8dff64/33258e3f7be8196d.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/324474/34/4746/15292/689f007bFa539bb50/62221ccd625a327b.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/315462/24/26709/19061/689f007bFabc484ea/c1bbb389dfb6ea35.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/328455/13/4928/14534/689f007cF88eec6ec/fd207ac81c0c253c.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/294220/34/22712/79694/689f007dF3e32d054/c4c5e0c592391ee9.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/309293/27/24316/12719/689f007dFfd63c7f7/3c6e47146a67a843.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/313526/12/21750/79358/689f007eF439431a4/9766d50a8798187c.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
