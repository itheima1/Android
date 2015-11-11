
### 涵盖Android方方面面的技术, 目前保持更新. 时刻与Android开发流行前沿同步.

------------------------------------------------------

### 目录

* [多媒体编程](#多媒体编程)
    - [图片加载库](#图片加载库)
    - [图片处理库](#图片处理库)
    - [图片加载相关博文](#图片加载相关博文)
    - [图片处理相关博文](#图片处理相关博文)
	- [视频相关](#)`-马上到来`

* [网络编程](#)`-马上到来`

* [数据处理](#)`-马上到来`
	- [数据解析/序列化](#)`-马上到来`
	- [数据库ORM](#)`-马上到来`

* [自定义控件](#)`-马上到来`

* [开发辅助](#)`-马上到来`

* [综合开发框架](#)`-马上到来`

* [其他三方](#)`-马上到来`

* [测试相关](#)`-马上到来`

### 注:
* 加星号*的为重点推荐
* 脑图地址: [戳这里](http://naotu.baidu.com/file/f1f87890d2b68684ed900ff639185ff0?token=1537e968b07153a4)

------------------------------------------------------
## 多媒体编程

### 图片加载库

> (解决网络, 文件, res, assets等图片的获取, 解析, 展示, 缓存等需求...)

名称 | 概要 | 详情
--- | --- | --- | ---
[*Picasso](https://github.com/square/picasso) | Github大神推荐的强大的图片下载和缓存库 | Square 开源的项目,主导者是 [JakeWharton](https://github.com/JakeWharton).
[*Glide](https://github.com/bumptech/glide) | Google推荐的图片加载和缓存的库 | 专注于平滑滚动时的流畅加载, Google开源项目, 2014年Google I/O 上被推荐
[*Fresco](https://github.com/facebook/fresco) | Facebook推荐的的Android图片加载库 | 自动管理图片的加载和图片的缓存.Facebook 在2015年上半年开源的图片加载库
[*Android-Universal-Image-Loader](https://github.com/nostra13/Android-Universal-Image-Loader) | 早期广泛使用的开源图片加载库 | 强大又灵活的Android库, 用于加载,缓存,显示图片.
[Volley](https://github.com/mcxiaoke/android-volley) | 2013年Google I/O推荐的网络通讯框架 | 使用volley加载网络图片，主要用到其中的ImageLoader, NetworkImageView类, 注意它不仅仅是个图片加载库.
[Cube-sdk](https://github.com/etao-open-source/cube-sdk) | 轻量级的Android开发框架 | 高效方便地加载网络图片, 更简易地处理网络API请求

### 图片处理库

> (解决图片缩放, 裁剪, 平移, 旋转等需求)

名称 | 概要 | 详情
--- | --- | --- | ---
[PinchImageView](https://github.com/boycy815/PinchImageView)|国人写的, 可能是体验最好的图片手势控件| 支持双击放大，双击缩小,超出边界会回弹, 滑动惯性，不同分辨率无缝切换，可与ViewPager结合使用。 star:360
[GestureViews](https://github.com/alexvasilkov/GestureViews)|包含ImageView的自定义FrameLayout | 项目目的是让图片的查看尽可能流畅平滑, 让开发者更加方便地集成到自己的应用中, 支持手势控制和动画 star:582
[*PhotoView](https://github.com/chrisbanes/PhotoView) | 致力于帮助开发者高效的创建可缩放的ImageView | 重写ImageView的实现, 支持多点触摸的图片缩放 star:4705
[subsampling-scale-image-view](https://github.com/davemorrissey/subsampling-scale-image-view) | 一个Android自定义图片视图, 专为图片画廊设计| 丰富的配置选项, 更方便的实现图片的手势缩放, 旋转, 平移. 无损展示大图, 完美的地嵌入画廊, 地图等.可显示大图(地图, 建筑设计图)等而不造成OutOfMemoryErrors(OOM内存溢出异常) star:1137
[TouchImageView](https://github.com/MikeOrtiz/TouchImageView) | 一个ImageView的拓展类 | 支持ImageView所有功能, 添加了平移, 缩放, 拖拽, 滑动, 双击缩放等动画.star:1252
[ImageViewZoom](https://github.com/sephiroth74/ImageViewZoom) | 自定义ImageView控件 | 一个可以缩放, 平移的自定义ImageView控件. star:1080

### 图片加载相关博文
##### [Picasso-强大的Android图片下载缓存库](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2014/0731/1639.html)
##### [Android的媒体管理框架:Glide 3.0发布](http://www.infoq.com/cn/news/2014/09/android-glide?utm_source=tuicool&utm_medium=referral)
##### [*开源选型之 Android 三大图片缓存原理、特性对比](http://mp.weixin.qq.com/s?__biz=MzAxNjI3MDkzOQ==&mid=400056342&idx=1&sn=894325d70f16a28bfe8d6a4da31ec304&scene=2&srcid=10210byVbMGLHg7vXUJLgHaR&from=timeline&isappinstalled=0#rd)
##### [Android Universal Image Loader 源码分析](http://a.codekk.com/blogs/detail/54cfab086c4761e5001b2540)
##### [Android DiskLruCache源码解析硬盘缓存的绝佳方案](http://blog.csdn.net/lmj623565791/article/details/47251585)
##### [android中图片的三级cache策略（内存、文件、网络）](http://blog.csdn.net/singwhatiwanna/article/details/9054001)

### 图片处理相关博文
##### [Android高效加载大图、多图解决方案，有效避免程序OOM](http://blog.csdn.net/guolin_blog/article/details/9316683)
##### [Android照片墙应用实现，再多的图片也不怕崩溃](http://blog.csdn.net/guolin_blog/article/details/9526203)
##### [Android多点触控技术实战，自由地对图片进行缩放和移动](http://blog.csdn.net/guolin_blog/article/details/11100327)
##### [Android 高清加载巨图方案 拒绝压缩图片](http://blog.csdn.net/lmj623565791/article/details/49300989)
##### [Android 优化Bitmap避免OutOfMemoryError](http://chjmars.iteye.com/blog/1157137)


