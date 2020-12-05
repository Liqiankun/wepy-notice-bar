![](https://github.com/Liqiankun/DLNoticeBar/blob/master/noticeBar.png)

[![npm package](https://nodei.co/npm/wepy-notice-bar.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/wepy-notice-bar)

## 说明
一个可以滚动的通知栏，在WEPY完美运行。支持多种样式，可以自定义滚动时间，延时，是否可关闭和图标自定义。

## 运行项目
```
npm install wepy-cli -g
wepy build --watch
```
更多关于Wepy请到[Wepy官方文档](https://wepyjs.github.io/wepy-docs/2.x/#/base/getstart)

## 安装
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
        leftIcon='../images/close.png'
      />
    </view>
  </view>
</template>

this.$invoke('NoticeBar', 'animate')
```
