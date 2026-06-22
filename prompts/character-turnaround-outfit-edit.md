# 角色三视图服饰替换：女篮球运动员

## 适用场景

当用户提供角色三视图 / 设定图，需要保持角色体型、头身比例、姿势、三视图结构、图片比例和整体构图不变，只替换服装、颜色、号码或配饰时，使用本案例。

## 当前参考图分析

- 类型：Q 版 / chibi 动漫角色三视图设定图。
- 视图结构：左侧正面、中央侧面、右侧背面，三个人物等距排列在白色背景上。
- 必须保持：头身比例、体型、脸型、发型、刘海、发夹、眼睛、站姿、手臂姿势、腿部比例、三视图布局、人物间距、白色背景、画布尺寸比例。
- 需要改变：把原服装替换为女篮球运动员服饰，红色篮球服，胸前和背后都有清晰球衣号码 `4`。
- 光影要求：柔和均匀光，不要明显方向光，不要强烈投影，不要高对比阴影。

## 通用 Prompt：三视图服装替换

```text
参考上传图片进行角色服装重绘，保持原图的三视图结构和画布比例不变：左侧为正面视图，中间为侧面视图，右侧为背面视图，三个人物的大小、间距、站姿和位置保持一致。保持角色原本的 Q 版头身比例、体型、脸型、发型、刘海、发夹、眼睛、表情、手臂姿势、腿部比例和整体轮廓不变，只替换服装。

将角色服装改为女篮球运动员服饰：红色篮球背心和红色篮球短裤，白色或浅色滚边，运动感材质，干净利落。正面视图的球衣胸前必须有清晰的白色号码 “4”；背面视图的球衣背后必须有清晰的白色大号码 “4”；侧面视图保持同一套红色篮球服结构。可以保留原角色的黑色长袜和运动鞋，也可以优化为适合篮球运动员的运动袜和球鞋，但不要改变腿部比例和角色体型。

画面保持干净的动漫角色设定图风格，白色或透明感浅色背景，线条清晰，颜色平整，细节干净。光影使用柔和均匀的无方向漫射光，不要明显从左、右、上、下照射的方向光，不要强烈投影，不要高对比阴影，不要戏剧化光影。整体像可用于角色建模或游戏角色设定的三视图参考图。

禁止改变三视图结构，禁止改变画布比例，禁止改变角色体型，禁止改变头身比例，禁止改变发型和脸，禁止改变站姿，禁止改变人物间距，禁止只画单人，禁止新增第四个视图，禁止强方向光，禁止强投影，禁止高对比阴影，禁止把篮球服改成其他颜色，禁止遗漏胸前 4 号，禁止遗漏背后 4 号，禁止乱码文字，禁止水印，禁止 logo，禁止背景复杂化。
```

## ChatGPT / GPT 绘图优化版

```text
Use the uploaded image as the reference for a character turnaround sheet. Preserve the original canvas aspect ratio and the three-view layout exactly: front view on the left, side view in the center, back view on the right. Keep the same chibi body proportions, body shape, head size, face, hairstyle, bangs, hair clips, eyes, expression, arm pose, leg proportions, standing pose, character scale, spacing, and plain white background. Change only the outfit.

Replace the current outfit with a female basketball player uniform: a red basketball jersey and red basketball shorts with clean white trim. The front view must show a clear white jersey number “4” on the chest. The back view must show a clear large white jersey number “4” on the back. The side view should show the same red basketball uniform from the side. Keep the outfit sporty, clean, and non-revealing. Socks and shoes can remain close to the original proportions, adjusted into athletic socks and basketball shoes if needed.

Use clean anime character-sheet rendering, crisp line art, flat clean colors, soft even ambient lighting, no directional lighting, no strong cast shadow, no dramatic contrast, no harsh highlights. The final image should look like a production-ready character turnaround reference sheet for a game character.

Do not change the three-view structure. Do not change the canvas aspect ratio. Do not change the body shape, proportions, hairstyle, face, pose, or spacing. No fourth view. No single-character crop. No complex background. No strong directional light. No harsh shadows. No high-contrast lighting. No wrong jersey color. Do not omit the number 4 on the front. Do not omit the number 4 on the back. No garbled text, no watermark, no logo.
```

## 输出规则

ChatGPT / GPT / nanobanana 默认不要单独拆出 Stable Diffusion 式 Negative Prompt。上面的中文和英文提示词已经把禁止项直接写进正文，复制整段使用即可。只有当平台明确提供 Negative Prompt 输入框，或用户明确要求时，才把禁止项单独拆出来。

## 测试记录 2026-06-22

### 测试 A：英文版 Prompt + GPT / 自动分辨率

- 结果：自动分辨率直接输出 1:1，导致三视图横向画布被压缩，人物比例明显变形。
- 分析：三视图角色设定图本质是宽画幅，原参考图接近 16:9。GPT 在自动分辨率下可能优先选择默认方图，导致三个角色被挤压在方形画布里，比例和间距漂移。

### 测试 B：英文版 Prompt + GPT / 16:9

- 结果：比自动分辨率好，但人物比例仍有轻微变形。
- 分析：英文版虽然写了 `Preserve the original canvas aspect ratio`，但没有把“不要方图、保持宽画布、保持三个人物横向占位和原始间距”放到足够靠前的位置；同时英文版更像通用编辑指令，可能让模型优先重绘服装而弱化画布比例和三视图几何约束。

### 测试 C：中文版 Prompt + gpt-image-2

- 结果：效果很好，没有明显比例变形。
- 可复用规律：中文提示词对当前工作流更稳定，尤其是“保持原图的三视图结构和画布比例不变”“三个人物的大小、间距、站姿和位置保持一致”“只替换服装”这些约束更直接。后续角色三视图换装优先使用中文提示词。

### 测试 D：同需求对比 nanobanana PRO

- 结果：GPT 画出来的效果比 nanobanana PRO 更好；nanobanana PRO 输出身体笔触偏重，精细度不如原图。
- 可复用规律：角色三视图换装、保持体型比例和干净设定图线条时，当前优先使用 GPT / gpt-image-2；nanobanana PRO 可作为备选，但需要额外强调“轻薄线条、不要厚重笔触、保持原图精细度”。

## gpt-image-2 推荐版：带画幅锁定

```text
参考上传图片进行角色服装重绘。必须保持原图的横向宽画布比例不变，保持与参考图一致的 16:9 横向构图；如果可以设置尺寸，使用 2048×1152 或同等 16:9 横向比例。不要输出 1:1 方图，不要裁切，不要拉伸，不要压缩人物，不要改变三个人物的横向间距。

保持原图的三视图结构不变：左侧为正面视图，中间为侧面视图，右侧为背面视图，三个人物的大小、间距、站姿和位置保持一致。保持角色原本的 Q 版头身比例、体型、脸型、发型、刘海、发夹、眼睛、表情、手臂姿势、腿部比例和整体轮廓不变，只替换服装。

将角色服装改为女篮球运动员服饰：红色篮球背心和红色篮球短裤，白色或浅色滚边，运动感材质，干净利落。正面视图的球衣胸前必须有清晰的白色号码 “4”；背面视图的球衣背后必须有清晰的白色大号码 “4”；侧面视图保持同一套红色篮球服结构。可以保留原角色的黑色长袜和运动鞋，也可以优化为适合篮球运动员的运动袜和球鞋，但不要改变腿部比例和角色体型。

画面保持干净的动漫角色设定图风格，白色或透明感浅色背景，线条清晰，颜色平整，细节干净。光影使用柔和均匀的无方向漫射光，不要明显从左、右、上、下照射的方向光，不要强烈投影，不要高对比阴影，不要戏剧化光影。整体像可用于角色建模或游戏角色设定的三视图参考图。

禁止改变三视图结构，禁止改变横向 16:9 画布比例，禁止输出 1:1 方图，禁止改变角色体型，禁止改变头身比例，禁止改变发型和脸，禁止改变站姿，禁止改变人物间距，禁止只画单人，禁止新增第四个视图，禁止强方向光，禁止强投影，禁止高对比阴影，禁止把篮球服改成其他颜色，禁止遗漏胸前 4 号，禁止遗漏背后 4 号，禁止乱码文字，禁止水印，禁止 logo，禁止背景复杂化。
```

## nanobanana PRO 补充约束

```text
在使用 nanobanana PRO 时，额外强调：保持原图轻薄干净线条和精细度，不要厚重笔触，不要粗糙笔刷，不要把身体阴影画得太重，不要增加过多肌肉线条或皮肤笔触，保持干净动漫三视图设定图质感。
```
