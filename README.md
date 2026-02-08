# 前言

随着我国城市化进程的不断推进，生活垃圾的分类与回收管理成为了一项重要的社会任务。基于微信小程序的社区垃圾回收管理系统SSM，旨在通过科技手段，提高居民垃圾分类意识，简化回收流程，促进环保行动的落实。以下是本项目的详细介绍。

## 内容介绍

本项目是一款基于微信小程序的社区垃圾回收管理系统，主要功能包括：用户注册登录、垃圾类别查询、预约回收、回收进度查询等。通过本系统，社区居民可以方便快捷地进行垃圾分类与回收，同时提高了回收效率，减轻了环保工作人员的负担。

## 技术介绍

本项目采用以下技术栈：

### 语言：
Java

### 使用框架：
Spring、SpringMVC、MyBatis、微信小程序

### 前端技术：
JS、Vue、CSS3、Uniapp

### 开发工具：
IDEA/Eclipse、Uniapp

### 数据库：
MySQL 5.7/8.0

### 数据库管理工具：
phpstudy/Navicat

### JDK版本：
jdk1.8

### Maven：
apache-maven 3.8.1-bin

### 前端环境：
Node.Js 12\14\16

## 核心代码

以下为项目中的一部分核心代码，展示如何实现垃圾类别查询功能：

```java
// Controller层
@RequestMapping("/getGarbageType")
@ResponseBody
public Result getGarbageType(String name) {
    List<GarbageType> list = garbageService.getGarbageType(name);
    if (list != null && list.size() > 0) {
        return new Result(true, "查询成功", list);
    } else {
        return new Result(false, "查询失败");
    }
}

// Service层
@Override
public List<GarbageType> getGarbageType(String name) {
    return garbageTypeMapper.getGarbageType(name);
}

// Mapper层
<select id="getGarbageType" parameterType="String" resultType="GarbageType">
    SELECT * FROM garbage_type WHERE name LIKE CONCAT('%', #{name}, '%')
</select>
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img14.360buyimg.com/ddimg/jfs/t1/342021/13/2889/80991/68c58287Ffd96f100/63c911da0786a50b.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/330219/4/13036/12551/68c5825fF9d6806d9/1b28167024f67134.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/348426/39/3058/12279/68c5825fFea8b3a21/d6b58637fd393575.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/342052/16/3139/14489/68c58260Ff5bb36e5/027531da1550e0d6.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/336174/39/10462/10166/68c58260F046d4b4f/c5f16591015a38c4.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/345661/2/2509/14907/68c58260F4cd66b96/5f74955f632d733e.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/333083/10/12910/12062/68c58261F3098d42a/3d1d3f36dc490596.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/329223/16/12883/14327/68c58261F28b5bb03/e3c94f84d899b878.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/334528/27/12969/15223/68c58261F34d8d0d5/139a0eade54af960.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/327334/3/19574/16616/68c58262F155afef0/a4690d591851dcc5.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
