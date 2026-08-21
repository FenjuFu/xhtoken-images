# xhtoken-images

Public image library for [`xhtoken-trending-content`](https://github.com/FenjuFu/xhtoken-trending-content)
（内容分发管线的配图库，与私仓的文案/记录分离）。

## 约定
- **文件名即标题**：用能描述图片内容的英文/拼音文件名（如 `en/llm-serving-throughput.png`），生成阶段的模型按文件名语义选图。
- 目录：`en/` 放英文渠道（X / Dev.to / Slack / Discord / Bluesky）用图；`zh/` 放知乎中文稿用图。
- 分发脚本按**文件名**核对回本库（不信任模型给的目录/host），正文图转 jsDelivr 国内优化镜像直链：
  `https://testingcf.jsdelivr.net/gh/FenjuFu/xhtoken-images@main/<path>`。

## 加新图
往本仓库 push 即可（本地目录 `D:\文档2\xhtoken-images`）。分发管线未配图或库里没有对应文件时，自动降级为纯文字发送。
