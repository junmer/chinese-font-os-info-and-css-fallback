# 中文排版常用字体 的 操作系统安装情况 和 CSS Fallback 方案 ![](https://img.shields.io/badge/release-no-red.svg?style=flat-square)


## 操作系统自带字体

**PC**

操作系统   | 宋体           | 黑体          | 楷体         | 仿宋体
--------- | ------------- | ------------ | ------------ | -------------
Win XP    | 宋体（SimSun）| 黑体（SimHei） | 楷体（Kaiti） | 仿宋（Fangsong）
Win 7     | 宋体（SimSun） | 黑体（SimHei）, 微软雅黑（Microsoft YaHei） | 楷体（Kaiti）| 仿宋（Fangsong）
Win 8     | 宋体（SimSun）, 新宋体（NSimSun）, 华文宋体（STSong）| 黑体（SimHei）, 华文细黑（STXihei）, 微软雅黑（Microsoft YaHei） | 楷体（Kaiti）, 华文楷体（STKaiti）| 仿宋（Fangsong）, 华文仿宋（STFangsong）
OS X      | 华文宋体（STSong）,儷宋 Pro（LiSong Pro）, 宋体 （SimeSun）| 冬青黑体简体中文 （Hiragino Sans GB）, 黑体 （Sime Hei）, 华文黑体（STHeiti）, 兰亭黑（LantingHei）, 儷黑 Pro（LiHei Pro） | 华文楷体（STKaiti）, 楷体（KaiTi）| 仿宋（FangSong）, 华文仿宋（STFangsong）

根据 [百度统计 - 操作系统份额报告](http://tongji.baidu.com/data/os) 排序, 截止 2015-5

**Mobile**

操作系统  | 宋体   | 黑体                       | 楷体         | 仿宋体
-------- | ----- | ------------------------- | ------------ | -------------
Android  | -     | Roboto, DroidSansFallback | -            | -
iOS      | -     | Heiti SC                  | -            | -


参考：[iosfonts](http://iosfonts.com/) , [Android Design - typography](http://developer.android.com/design/style/typography.html)


**待完善**

- 简体, 繁体 未详细说明
- Linux, Ubuntu 系统未覆盖

## CSS Fallback

- 宋体

```
font-family: SimSun, '宋体', STSong, 'Arial Narrow', serif;
```

- 黑体

```
font-family: Helvetica, 'Hiragino Sans GB', 'Microsoft Yahei', '微软雅黑', Arial, sans-serif;
```

- 楷体

```
font-family: KaiTi, '楷体', STKaiti, '华文楷体', serif;
```

- 仿宋体

```
font-family: FangSong, '仿宋', STFangSong, '华文仿宋', serif;
```

