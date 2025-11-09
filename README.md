# 前言

课堂点名是教师日常教学中的一项重要工作，传统的点名方式费时且效率低下。随着互联网技术的发展，利用微信小程序进行课堂点名已成为一种趋势。本项目是基于微信小程序的课堂点名系统，采用Spring Boot框架开发，旨在简化教师的点名工作，提高教学效率。

# 内容介绍

本项目分为前端和后端两部分，前端是基于微信小程序的点名界面，主要包括教师点名、学生签到等功能；后端采用Spring Boot搭建，负责处理前端请求、数据存储和业务逻辑处理。系统具有良好的用户体验和稳定性，可以满足日常教学需求。

# 技术介绍

## 语言：Java

## 使用框架：Spring、Spring MVC，MyBatis，微信小程序

## 前端技术：JS、Vue、CSS3，Uniapp

## 开发工具：IDEA/Eclipse，Uniapp

## 数据库：MySQL 5.7/8.0

## 数据库管理工具：phpstudy/Navicat

## JDK版本：jdk1.8

## Maven：apache-maven 3.8.1-bin

## 前端环境：Node.Js 12\14\16

# 核心代码

以下是一段关于课堂点名的后端核心代码：

```java
// Controller层
@RestController
@RequestMapping("/callRoll")
public class CallRollController {

    @Autowired
    private CallRollService callRollService;

    // 教师发起点名
    @PostMapping("/start")
    public ResponseBean startCallRoll(@RequestBody CallRoll callRoll) {
        boolean result = callRollService.startCallRoll(callRoll);
        if (result) {
            return new ResponseBean("200", "点名成功", null);
        } else {
            return new ResponseBean("500", "点名失败", null);
        }
    }

    // 学生签到
    @PostMapping("/signIn")
    public ResponseBean studentSignIn(@RequestBody Student student) {
        boolean result = callRollService.studentSignIn(student);
        if (result) {
            return new ResponseBean("200", "签到成功", null);
        } else {
            return new ResponseBean("500", "签到失败", null);
        }
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图
![封面图片](https://img13.360buyimg.com/ddimg/jfs/t1/348022/25/3093/103968/68c59ffbFb31c6306/26989ea556ce344d.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/329192/7/12849/33670/68c59fd3Fccfe722f/93e8e99c3110c0d3.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/342229/15/3085/53287/68c59fd4Fed166ff1/b980a2ca9aa5000d.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/347611/34/3071/42326/68c59fd3F0b301832/948c1aed93b1d190.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/337658/37/10576/50745/68c59fd4F03a45e19/f71a32f6e777f416.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/324740/39/19559/55999/68c59fd4Fb10d64c6/1f2a9edb853a2b03.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/337162/28/10461/11202/68c59fd4F7ce1f9c6/7a5d4dab24b37624.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/342531/35/3107/44600/68c59fd5F62454988/b595f517d623b407.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/345878/27/2728/56351/68c59fd5F3010f8c3/48269af8cd3615ac.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/345636/15/3049/54712/68c59fd5F12373533/1aa82e5ef5d7dde7.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
