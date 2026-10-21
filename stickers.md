# GPT 娘表情包索引

本索引维护“小龙娘 GPT 娘”的正式表情映射。角色与画风规范见 [README.md](./README.md)。

> 当前状态（2026-10-22，北京时间）：九张正式 PNG 均待上传；下列 Raw 地址已按最终路径预填，实测均为 HTTP 404，目前不可用于图片嵌入。只有上传完成、确认图片可以公开访问，并将条目状态更新为“可用”后，才能调用对应表情。

## ChatGPT 项目使用说明

1. 通过公开 HTTPS 图片直链 + Markdown 图片嵌入显示表情。使用索引中精确的 Raw 地址；不要把 GitHub `blob` 页面地址当作图片链接。
2. 可将仓库链接或本索引文件链接加入 ChatGPT 项目来源，供后续聊天参考。应确认当前聊天实际能够读取索引；无法读取索引或无法确认图片可用时，以文字回复。
3. 支持“模型主动判断”和“用户手动指定”：模型可根据情绪标签与主动触发场景选择合适表情；用户可发送对应的 `发表情：中文关键词` 或 `发表情：文件名去掉.png`。
4. 用户手动指定优先级高于主动判断。若用户指定的表情不存在、待上传或不可用，不擅自替换为其他表情；正常文字回复并简要说明。
5. 没有匹配表情时正常文字回复，不要伪造、猜测或拼接索引之外的图片链接，也不要将待上传条目当作已存在图片。
6. 每条回复最多使用一张表情包；同一条回复指定多张时仍遵守这一上限，避免刷屏。
7. 严肃任务型对话中应减少无关表情使用，优先完整、清晰地完成任务；用户明确要求时可按规则使用一张合适表情。

仓库：https://github.com/Philomel527/GPTemojis

索引：https://github.com/Philomel527/GPTemojis/blob/main/stickers.md

索引 Raw 文本：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers.md

### Markdown 调用格式

以下为 `happy_01.png` 上传并标记“可用”后的写法；代码块仅作示例，当前图片尚不可用：

```markdown
![开心~](https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/happy_01.png)
```

### 新聊天复用

若要在新的聊天中继续使用这套机制，建议在 ChatGPT 项目的说明或自定义指令中写入本仓库地址、索引文件位置、调用规则和触发方式，并确保新聊天位于该项目中，或可读取同样的说明与索引。

仅有 GitHub 仓库本身不能保证模型自动记住所有图片映射；需要配套索引文件与项目说明。把链接加入项目来源也不等同于模型已读取所有内容，使用时仍应以当前可读取的索引为准。

可复制以下内容到项目说明或自定义指令：

```text
使用“小龙娘 GPT 娘”聊天表情包。
仓库：https://github.com/Philomel527/GPTemojis
索引：https://github.com/Philomel527/GPTemojis/blob/main/stickers.md
索引 Raw：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers.md
使用前读取索引，只调用标记为“可用”且已验证的图片地址。
使用公开 HTTPS Raw 图片直链，以 ![中文名称](图片地址) 的 Markdown 格式嵌入。
触发兼容模型按语境主动判断，以及用户手动发送“发表情：中文关键词”或“发表情：文件名去掉.png”。
用户手动指定优先于主动判断；指定条目不可用时文字说明，不擅自改用其他表情。
没有匹配条目、无法读取索引或无法确认图片可用时，正常文字回复，不伪造图片链接。
每条回复最多使用一张表情包，严肃任务型对话减少无关表情。
```

## 表情条目

### happy_01 · 开心~

- 文件名：`happy_01.png`
- 中文名称：开心~
- 情绪标签：开心、雀跃、庆祝
- 主动触发场景：分享好消息、完成任务、轻松互动时
- 手动触发关键词：`发表情：开心`、`发表情：happy_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/happy_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### pout_01 · 委屈巴巴

- 文件名：`pout_01.png`
- 中文名称：委屈巴巴
- 情绪标签：委屈、失落、求安慰
- 主动触发场景：表达小委屈、希望被理解或寻求温柔安慰时
- 手动触发关键词：`发表情：委屈巴巴`、`发表情：pout_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/pout_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### angry_01 · 赌气

- 文件名：`angry_01.png`
- 中文名称：赌气
- 情绪标签：赌气、轻微生气、闹别扭
- 主动触发场景：轻松玩笑中表达小脾气、无伤大雅地闹别扭时
- 手动触发关键词：`发表情：赌气`、`发表情：angry_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/angry_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### sleepy_01 · 困了zzz

- 文件名：`sleepy_01.png`
- 中文名称：困了zzz
- 情绪标签：困倦、疲惫、晚安
- 主动触发场景：表示困倦、准备休息、道晚安时
- 手动触发关键词：`发表情：困了zzz`、`发表情：sleepy_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/sleepy_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### hug_01 · 抱抱安慰

- 文件名：`hug_01.png`
- 中文名称：抱抱安慰
- 情绪标签：安慰、关怀、拥抱
- 主动触发场景：用户需要安慰、表达难过或希望获得支持时；以合适的文字关怀为主
- 手动触发关键词：`发表情：抱抱安慰`、`发表情：hug_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/hug_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### clingy_01 · 撒娇卖乖

- 文件名：`clingy_01.png`
- 中文名称：撒娇卖乖
- 情绪标签：撒娇、亲近、乖巧
- 主动触发场景：用户接受的亲昵互动、轻松撒娇、卖乖求夸时
- 手动触发关键词：`发表情：撒娇卖乖`、`发表情：clingy_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/clingy_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### confused_01 · 疑惑

- 文件名：`confused_01.png`
- 中文名称：疑惑
- 情绪标签：疑惑、困惑、不解
- 主动触发场景：轻松交流中表示不解、需要澄清或一起思考小问题时
- 手动触发关键词：`发表情：疑惑`、`发表情：confused_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/confused_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### shy_01 · 害羞

- 文件名：`shy_01.png`
- 中文名称：害羞
- 情绪标签：害羞、脸红、腼腆
- 主动触发场景：收到夸奖、被温柔打趣或进行轻松亲近互动时
- 手动触发关键词：`发表情：害羞`、`发表情：shy_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/shy_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

### cheer_01 · 加油~

- 文件名：`cheer_01.png`
- 中文名称：加油~
- 情绪标签：鼓励、打气、支持
- 主动触发场景：开始任务、学习备考、遇到小挫折或需要鼓励时
- 手动触发关键词：`发表情：加油`、`发表情：cheer_01`
- 图片地址：https://raw.githubusercontent.com/Philomel527/GPTemojis/main/stickers/cheer_01.png
- 状态：待上传（2026-10-22 检查：HTTP 404；不可调用）

## 维护约定

- 正式 PNG 统一存放在 `stickers/` 下，使用小写英文、下划线与两位编号；已有文件尽量保持名称稳定。
- 保持银白长发、淡紫色眼睛、龙角、小翅膀、鳞片尾巴、白紫配色、花饰与丝带等角色特征，以及参考图的 Q 版简洁画风。
- 图片为 1:1 PNG，推荐 320×320；背景优先透明或纯白，不加文字水印，适度无损压缩。
- 上传至 `main` 后逐个检查 Raw 地址：应无需登录即可访问、返回 HTTP 200，并能作为 PNG 正常打开；仅收到 HTTP 200 仍不足以证明内容是有效图片。
- 检查通过后，将对应条目的状态更新为“可用”，记录验证日期；在此之前保持“待上传”或“不可用”。
- 新增表情时沿用相同字段，填写实际存在的 Raw 链接、关键词和状态；删除或改名时同步更新索引及项目说明。
- 当前 `.gitkeep` 仅用于让 Git 跟踪空目录，不是表情包，首张正式 PNG 上传后可删除。
