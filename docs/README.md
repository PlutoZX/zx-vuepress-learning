# Hello zhaoxuan

## 静态资源
相对目录下的图片
![An image](./WechatIMG2.jpg)


public下的图片，public下的静态资源地址基于config.js里的base设置，如果配置项变了就会出错，可以用$withBase修改
![An image](/WechatIMG2.jpg)


通过$withBase修正路径的图片
<img :src="$withBase('/WechatIMG2.jpg')" alt="foo">

## 链接
[京东](https://www.jd.com/) is best netsite.

## Title3

---
title: Blogging Like a Hacker
lang: en-US
---

---
meta:
  - name: description
    content: hello
  - name: keywords
    content: super duper SEO
---


## GitHub-Style Tables

| 接口地址                         | 入参名称           | 入参类型       | 入参描述             |
| ------------------------------ |:-----------------:| :------------:|--------------------:|
| /freeway/queryOpenStatus       |
|                                | success           |   String      |是否成功               |
|                                | code              |   String      |返回码               |



## Emoji
:tada: :100:



## Table of Contents
[[toc]]


## Custom Containers
::: tip 正常
This is a tip
:::

::: warning 警告
This is a warning
:::

::: danger 禁止
Danger zone, do not proceed
:::


## Code Block
``` js{4}
// 数字代表高亮行数
export default {
  data () {
    return {
      msg: 'Highlighted!'
    }
  }
}
```

``` js{1}
if(a){
    console.log(a);
}else if(b){
    console.log)(b);
}
```


## 在markdown中使用vue
### 差值语法
1 + 1 = {{1 + 1}}
<div v-for="i in 3">{{ i }} </div>

### 页面元数据
{{ $page }}

### 语法不编译直接输出
::: v-pre
`{{ This will be displayed as-is }}`
:::

::: v-pre
{{ 1 + 1}}
:::

### 使用vue组件
<test-demo/>