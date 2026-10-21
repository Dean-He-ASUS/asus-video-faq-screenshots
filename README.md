# ASUS 路由器视频图文教程 · 截图图床

本仓库存放 **ASUS 官方支持视频教程**转制的图文 FAQ 截图，用于 52asus 论坛
（https://www.52asus.com/）的图文教程转载帖**热链引用**。

## 用途

52asus 是 Discuz 论坛，站点的服务端附件存储当前不可写（上传接口返回 aid，
但回读提示「该附件无法读取」），因此图文教程的截图无法走 Discuz 附件。
本站既有转载文章统一采用**热链**方式引用图片，本仓库即为此提供稳定、
无防盗链、可直接 `<img src>` 引用的图片地址。

## 目录结构

```
<视频ID>/step_XX.jpg     截图，按视频 ID 归档
```

`<视频ID>` 为 YouTube 视频 ID，与 `D:\FAQ_Bot\FAQ.xlsx`「ASUS SUPPORT LINK」
列一一对应。

## 引用方式

原始地址：

```
https://raw.githubusercontent.com/Dean-He-ASUS/asus-video-faq-screenshots/main/<视频ID>/step_XX.jpg
```

CDN 加速（推荐，读者侧更快）：

```
https://cdn.jsdelivr.net/gh/Dean-He-ASUS/asus-video-faq-screenshots@main/<视频ID>/step_XX.jpg
```

论坛正文用 Discuz BBCode：

```
[img]https://cdn.jsdelivr.net/gh/Dean-He-ASUS/asus-video-faq-screenshots@main/<视频ID>/step_XX.jpg[/img]
```

## 版权

截图取自 ASUS 官方支持视频（youtube.com/@ASUS），版权归 ASUS 所有。
转载用途请遵守 ASUS 与 52asus 论坛的相关规定。

## 相关工具

上传与正文改写工具位于 FAQBot 项目：

- `tools/upload_hotlink_images.py` — 批量上传截图、生成 URL 映射、
  把正文 `[attach]N` 改写为 `[img]热链URL[/img]`、逐图回取校验
- `tools/import_video_faq.py` — 把图文 FAQ 注册进 FAQBot 待转载池
