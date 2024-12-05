# MDC-NG

成人电影数据采集工具

![MDC-NG](https://file.lifebus.top/imgs/mdc_ng_cover.png)

![](https://img.shields.io/badge/%E6%96%B0%E7%96%86%E8%90%8C%E6%A3%AE%E8%BD%AF%E4%BB%B6%E5%BC%80%E5%8F%91%E5%B7%A5%E4%BD%9C%E5%AE%A4-%E6%8F%90%E4%BE%9B%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81-blue)

## 应用简介

### 视频刮削整理

支持硬链接、软链接、复制、移动、原地整理等多种整理方式

+ 识别影片ID
+ 抓取元数据
+ 创建目标目录
+ 下载、处理图片
+ 整理视频以及自带的字幕文件到目标目录
+ 生成nfo文件

### 目录监控

> 监控开启后不会刮削目录内的存量视频，只会对新文件的创建做出响应

当你的媒体目录是本地盘时，优先使用性能模式来获得最佳体验。其他情况或遇到目录监控不工作，请改成兼容模式

提供两种监控模式针对不同场景：

#### 性能模式

监听系统级文件变更事件，即时响应，性能最好。但不支持网盘、NAS等挂载到本地的目录

#### 兼容模式

定时检查文件更新，性能一般，响应有一定延迟。优点是不依赖系统事件，兼容性强

### 演员刮削

+ 目前支持emby服务端刮削
+ 刮削信息源：维基百科
+ 刮削图片源：graphis，gfriends；其中graphis源的图片质量优秀并且有背景图，作为首选
+ graphis网站有演员早期到最近时期的照片，目前默认刮削早期照片（比较青春..)，后续版本更新会添加为可选项
+ gfriends是社区维护的演员头像数据库，质量参差不齐，但覆盖范围宽，能够作为graphis很好的补充。该数据在后端初始化时会进行缓存，重启服务会检查数据更新。后续会添加定时检查功能

## 应用特性

+ WebUI交互界面
+ 高性能、高质量刮削器，多刮削源同步抓取元数据，支持多种整理方式。目前已经支持近20个高质量刮削源，新源适配陆续添加中
+ 支持多目录监控，检测到新文件自动刮削入库
+ 手动存量整理
+ 联动Emby演员信息、图片刮削
+ 图片自动添加标签、多引擎文本翻译、内置演员数据库、sehuatang标题数据库等等

---

![Ms Studio](https://file.lifebus.top/imgs/ms_blank_001.png)