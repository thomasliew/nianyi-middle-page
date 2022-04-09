---
title: css3方式实现元素居中
date: 2022-04-09 21:10:50
tags: css
---

## 前言

平时经常接触一些场景需要将元素居中,  
css3提供了简单的方式来实现.

## 垂直居中

``` html
<div class="parent" style="height:700px;">  
    <div class="child" style="height:200px;width:300px; left:5%"></div>  
    <div class="child" style="height:300px;width:300px; left:60%;"></div>  
</div>  
```

``` css {6}
.parent{  
    background-color: wheat;
    position:relative;
}  
.child{  
    transform: translateY(-50%);  
    border:solid 1px red;
    display:inline-block;
    position: absolute;
    top:50%;
}  
```

## 垂直水平均居中

> 若需要xy均居中,将上面高亮部分替换为如下代码.

``` css
transform: translate(-50%,-50%);
```
