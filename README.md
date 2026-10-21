# GPTemojis

“小龙娘 GPT 娘”的聊天表情包仓库，供 ChatGPT 项目通过公开 HTTPS 图片直链与 Markdown 图片嵌入显示表情。

## 目录与文件

- `stickers/`：存放所有正式表情包 PNG。图片未补齐时以 `.gitkeep` 保留目录，首张正式图片上传后可删除该占位文件。
- [`stickers.md`](./stickers.md)：表情索引，记录文件名、中文名称、情绪标签、触发场景、手动关键词、Raw 图片直链及可用状态。
- `README.md`：仓库说明、角色与图片规范、维护方式。

正式资源的目标结构如下（不代表图片已经上传）：

```text
GPTemojis/
├── README.md
├── stickers.md
└── stickers/
    ├── happy_01.png
    ├── pout_01.png
    ├── angry_01.png
    ├── sleepy_01.png
    ├── hug_01.png
    ├── clingy_01.png
    ├── confused_01.png
    ├── shy_01.png
    └── cheer_01.png
```

## 角色与图片规范

- 固定角色：银白长发、淡紫色眼睛、龙角、小翅膀、鳞片尾巴；采用白紫色系、花饰与丝带，气质精致、柔和、可爱，带一点书卷气。
- 统一参考仓库已确认的[“哭哭”表情包](./gpt%E5%93%AD%E5%93%AD_320x320.png)，保持 Q 版比例、简洁线条、清晰情绪及一致的角色设定。
- 所有正式图片均为 1:1 方图，推荐 320×320，PNG 格式；优先透明或纯白背景，不使用复杂场景、文字或水印。
- 优先使用无损 PNG 优化压缩体积，检查缩小后仍清晰；保留透明度，避免明显画质损失。

## 发布与维护

仓库应保持 **Public**，正式图片放在 `main` 分支的 `stickers/` 下，以便无需登录即可通过公开 HTTPS 直链访问。固定格式为：

```text
https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/文件名.png
```

新增或替换图片时，保持文件名与索引同步；逐个确认 Raw 地址返回 HTTP 200、内容为可打开的 PNG，再将对应索引状态改为“可用”。尚未上传、校验失败或标记为待上传的条目不得用于聊天嵌入。GitHub 的 `blob` 页面不是图片直链。

## ChatGPT 项目使用说明

完整调用规则、Markdown 示例及可复制到项目说明中的配置见 [`stickers.md`](./stickers.md#chatgpt-项目使用说明)。支持模型主动判断与用户手动指定，手动指定优先；每条回复最多一张，无匹配或图片不可用时正常文字回复，不伪造链接；严肃任务型对话应减少无关表情。

可将[仓库链接](https://github.com/Philomel527/GPTemojis)或[索引文件链接](https://github.com/Philomel527/GPTemojis/blob/main/stickers.md)加入 ChatGPT 项目来源。在新聊天中复用时，应同时在项目说明或自定义指令中写入仓库地址、索引位置、调用规则和触发方式。仅有仓库本身不能保证模型自动记住图片映射，需要配套索引文件与项目说明。

## 当前资源状态

截至 2026-10-22（北京时间），仓库已为 Public，默认分支为 `main`；原有“哭哭”参考图保留在根目录。清单中的九张正式 PNG 尚未上传，九个预留 Raw 地址实测均返回 HTTP 404。本文与索引先行准备，当前 `stickers/` 使用 `.gitkeep` 占位；补齐图片并逐一验证后再启用。
