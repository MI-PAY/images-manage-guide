## 想方设法不使用图片
网页中占据流量大头的就是图片，基本占据50%以上，而活动页或产品展示页基本都在90%以上
* 使用字体实现icon图片，可以按需加载字体，做到最小化
	* 按需下载字体（http://www.iconfont.cn/plus/collections/index）
	* 详细的使用说明（http://www.alloyteam.com/2015/05/%E6%B5%85%E5%B0%9Diconfont/）
* 通过纯css实现一些icon图标，如箭头，对勾，×等等
	* http://cssicon.space/
	* http://saeedalipoor.github.io/icono/

## 色彩和层次简单的用png格式（如logo图片），反之用jpg图片（如产品类）
png格式非常适合处理色彩和层次相对单一的图片，反之jpg格式更加适合，格式用对了，可以保证相同大小情况下图片更加清晰，或者相同清晰度下图片更小
* 引用：
	* http://www.cnblogs.com/chenguiya/p/3216909.html
	* http://www.bjseoguwen.com/article/20160314164259.html

## 图片尺寸
* icon,logo类单张图片尽量保持`5k`
* 产品类图片尽量保持在`20k`

## 使用雪碧图（即多张图片合并成一张）
* 合并多张图片可以减少http请求次数，因为建立连接也是耗时的瓶颈
* 多张图片合并之后，往往是单张图片总和的一半还少

## 使用gulp脚手架工具批量自动化压缩处理
* 详情请参考：https://github.com/chenky/gulp

## 使用延迟加载
* 首屏显示比不需要一次把所有图片加载出来，只需要加载部分即可
* 注意js脚本也占流量请求，所以要在图片大小和js大小中做权衡
* lazyload脚本地址
	* https://raw.githubusercontent.com/tuupola/jquery_lazyload/master/jquery.lazyload.js(http://www.appelsiini.net/projects/lazyload)

## 使用webp图片
* 目前京东和天猫，腾讯都在使用此种格式图片
* 1、若使用场景是浏览器，可以：
	* JavaScript 能力检测，对支持 WebP 的用户输出 WebP 图片
	* 使用 WebP 支持插件：WebPJS(http://webpjs.appspot.com/) 
* 2、若使用场景是 App，可以：
	* Android 4.0 以下 WebP 解析库
	* iOS WebP 解析库
* 3、转换工具：
	* 智图（http://zhitu.tencent.com/）
	* iSparta（http://isparta.github.io/）
