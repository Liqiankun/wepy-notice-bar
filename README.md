![](https://github.com/Liqiankun/DLNoticeBar/blob/master/noticeBar.png)

## 说明
一个可以滚动的通知栏，在WEPY完美运行。支持多种样式，可以自定义滚动时间，演示，是否可关闭和图标。

## 运行项目
```
npm install wepy-cli -g
wepy build --watch
```
更多关于Wepy请到[Wepy官方文档](https://tencent.github.io/wepy/document.html#/)

## 安装（马上支持）
```
npm install wepy-notice-bar --save
```

## 使用
```
import NoticeBar from 'wepy-notice-bar'

<template>
  <view class="container">
    <view class='cell-ctn'>
      <text>普通通告栏</text>
      <NoticeBar
        :text.sync='text'
        :leftIcon.sync='leftIcon'
      />
    </view>
  </view>
</template>

this.$invoke('NoticeBar', 'animate')
```
