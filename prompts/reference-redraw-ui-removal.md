# 参考图重绘去 UI：废弃建筑游戏地图场景

## 适用场景

当参考图是带 UI 的 2D / 像素风游戏截图，需要保留场景布局、建筑与道路关系、植被分布和传统正交斜俯视游戏视角，同时去掉所有界面元素并改成指定美术风格时，使用本案例。

## 参考图内容分析

- 场景：废弃或半废弃的现代小屋 / 实验室建筑外部，建筑位于画面中右侧，顶部可见浅蓝色地砖房间，外部有门廊、墙体、窗户和设备箱。
- 地形：泥土道路从左下向中间延伸，再分叉到右侧和建筑入口周围，周围大面积绿色草地。
- 植被：多棵果树和大树分布在左侧、右侧和边缘区域，草丛、灌木、野花、杂草围绕道路与建筑生长。
- 道具：建筑内外有纸张、箱子、设备、石块、杂物和门口小装置。
- 角色：小型玩家角色位于建筑入口附近，可按需求保留为小比例 NPC / 冒险者，或移除。
- 必须移除：版本号、帧率文字、bilibili 水印、教学提示文本、准星、血条、技能卡、快捷栏、背包提示、播放按钮等所有 UI / HUD / 水印 / 叠加文字。

## 可复制 Prompt：通用占位版

```text
参考上传图片进行重绘，保留原图中的场景结构、空间布局、建筑位置、道路走向、草地范围、树木和灌木分布、石块与杂物的大致位置。保留画面中右侧的废弃现代小屋 / 实验室建筑、可见屋顶与室内地砖区域、入口门廊、泥土道路、周围草地、果树、杂草、灌木和零散道具。去掉所有游戏 UI、HUD、文字、水印、版本号、帧率、教学提示、准星、血条、技能栏、快捷栏、背包图标、播放按钮和任何叠加界面元素，只保留干净的游戏场景地图。

保持传统 2D 游戏地图视角：固定正交斜俯视镜头，三分之四俯视角，相机从上方向下约 45 度观察，使用正交投影 / 平行投影，不使用透视投影。地面占主要画面，建筑显示顶部，同时露出少量前立面和侧立面，整体像经典 JRPG / 手游地图场景，空间清晰、可读性强，没有明显近大远小。

将画面风格改为【目标风格】。使用【色彩关键词】色调，营造【氛围关键词】氛围。材质表现为【材质关键词】，细节精致但不要破坏原图地图布局。整体是高完成度 2D 手绘游戏场景背景，画面干净、层次清楚、道具分布自然，适合作为游戏地图场景资源。

禁止改变视角，禁止改变主要布局，禁止平视，禁止低角度，禁止仰视，禁止电影镜头，禁止广角畸变，禁止鱼眼，禁止强透视，禁止明显近大远小，禁止纯 90 度顶视图，禁止航拍照片，禁止真实摄影感，禁止海报式构图，禁止添加 UI，禁止添加文字，禁止水印，禁止 logo。
```

## 可复制 Prompt：治愈日系幻想手游风

```text
参考上传图片进行重绘，保留原图中的场景结构、空间布局、建筑位置、道路走向、草地范围、树木和灌木分布、石块与杂物的大致位置。保留画面中右侧的废弃现代小屋 / 实验室建筑、可见屋顶与浅蓝色室内地砖区域、入口门廊、泥土道路、周围草地、果树、杂草、灌木、野花和零散道具。去掉所有游戏 UI、HUD、文字、水印、版本号、帧率、教学提示、准星、血条、技能栏、快捷栏、背包图标、播放按钮和任何叠加界面元素，只保留干净的游戏场景地图。

保持传统 2D 游戏地图视角：固定正交斜俯视镜头，三分之四俯视角，相机从上方向下约 45 度观察，使用正交投影 / 平行投影，不使用透视投影。地面占主要画面，建筑显示屋顶和室内顶部结构，同时露出少量前立面和侧立面，整体像经典 JRPG / 手游地图场景，空间清晰、可读性强，没有明显近大远小。

将画面风格改为治愈日系幻想手游风格，2D 手绘游戏场景，温馨废弃小屋探索地图，低饱和蓝绿色调，柔和赛璐璐阴影，清晨柔光，轻微绘本质感，草地蓬松自然，树冠圆润，建筑边缘干净，杂物精致但不杂乱，带一点安静神秘的冒险氛围。整体是高完成度 2D 手绘游戏场景背景，画面干净、层次清楚、道具分布自然，适合作为游戏地图场景资源。

禁止改变视角，禁止改变主要布局，禁止平视，禁止低角度，禁止仰视，禁止电影镜头，禁止广角畸变，禁止鱼眼，禁止强透视，禁止明显近大远小，禁止纯 90 度顶视图，禁止航拍照片，禁止真实摄影感，禁止海报式构图，禁止添加 UI，禁止添加文字，禁止水印，禁止 logo，禁止保留血条、技能栏、快捷栏、教学提示、版本号、bilibili 水印和播放按钮。
```

## Negative Prompt / 负面提示词

```text
UI, HUD, interface, game overlay, health bar, skill icons, quickslot, inventory icon, crosshair, tutorial text, subtitle, watermark, logo, bilibili watermark, version text, fps text, play button, text overlay, eye-level view, low angle, worm’s-eye view, cinematic camera, wide-angle lens, fisheye lens, strong perspective, vanishing point perspective, obvious perspective scaling, tilted camera, realistic photography angle, poster composition, pure 90-degree top-down view, aerial photography, realistic architectural photography, excessive depth perspective, blurry, low quality, messy layout
```

## 测试记录 2026-06-17

### 测试 A：韩漫奇幻 RPG 场景风（GPT 绘图）

- 结果：出现噪点，整体效果不好。
- 初步判断：`韩漫奇幻 RPG`、`梦幻蓝绿色彩`、`细腻建筑细节` 容易让 GPT 在手绘背景里增加颗粒、脏点、过密纹理或不稳定的噪声细节。
- 后续调整：GPT 绘图时，如果目标是干净游戏地图，应减少“梦幻”“细腻复杂”的堆叠，改用“干净色块、柔和赛璐璐阴影、低噪点、无颗粒、边缘清晰、平滑渐变、不要纹理噪声”。

### 测试 B：治愈日系幻想手游风（GPT 绘图）

- 结果：效果还可以，没有出太大问题。
- 可复用规律：`治愈日系幻想手游风`、`低饱和蓝绿色调`、`柔和赛璐璐阴影`、`清晨柔光`、`轻微绘本质感`、`画面干净、层次清楚` 对 GPT 更稳定。

### 测试 C：治愈日系幻想手游风（nanobanana PRO 绘图）

- 结果：效果不错，整体质量比 GPT 更高。
- 可复用规律：同一套参考图重绘提示词在 nanobanana PRO 上可以保留更高完成度；后续可优先用 nanobanana PRO 做最终高质量版本，用 GPT 做结构和风格验证。

## GPT 去噪优化版 Prompt：治愈日系幻想手游风

```text
参考上传图片进行重绘，保留原图中的场景结构、空间布局、建筑位置、道路走向、草地范围、树木和灌木分布、石块与杂物的大致位置。保留画面中右侧的废弃现代小屋 / 实验室建筑、可见屋顶与浅蓝色室内地砖区域、入口门廊、泥土道路、周围草地、果树、杂草、灌木、野花和零散道具。去掉所有游戏 UI、HUD、文字、水印、版本号、帧率、教学提示、准星、血条、技能栏、快捷栏、背包图标、播放按钮和任何叠加界面元素，只保留干净的游戏场景地图。

保持传统 2D 游戏地图视角：固定正交斜俯视镜头，三分之四俯视角，相机从上方向下约 45 度观察，使用正交投影 / 平行投影，不使用透视投影。地面占主要画面，建筑显示屋顶和室内顶部结构，同时露出少量前立面和侧立面，整体像经典 JRPG / 手游地图场景，空间清晰、可读性强，没有明显近大远小。

将画面风格改为治愈日系幻想手游风格，2D 手绘游戏场景，温馨废弃小屋探索地图，低饱和蓝绿色调，柔和赛璐璐阴影，清晨柔光，干净色块，平滑渐变，边缘清晰，草地蓬松自然，树冠圆润，建筑边缘干净，杂物精致但不杂乱，带一点安静神秘的冒险氛围。整体是高完成度 2D 手绘游戏场景背景，画面干净、低噪点、无颗粒感、无脏污纹理、层次清楚、道具分布自然，适合作为游戏地图场景资源。

禁止改变视角，禁止改变主要布局，禁止平视，禁止低角度，禁止仰视，禁止电影镜头，禁止广角畸变，禁止鱼眼，禁止强透视，禁止明显近大远小，禁止纯 90 度顶视图，禁止航拍照片，禁止真实摄影感，禁止海报式构图，禁止添加 UI，禁止添加文字，禁止水印，禁止 logo，禁止保留血条、技能栏、快捷栏、教学提示、版本号、bilibili 水印和播放按钮，禁止噪点，禁止颗粒，禁止脏污纹理，禁止过度锐化，禁止杂色斑点，禁止随机纹理，禁止画面发灰。
```

## GPT 负面提示词补强

```text
UI, HUD, interface, game overlay, health bar, skill icons, quickslot, inventory icon, crosshair, tutorial text, subtitle, watermark, logo, bilibili watermark, version text, fps text, play button, text overlay, noise, grain, speckles, dirty texture, random texture, over-sharpening, muddy colors, gray cast, messy micro details, eye-level view, low angle, worm’s-eye view, cinematic camera, wide-angle lens, fisheye lens, strong perspective, vanishing point perspective, obvious perspective scaling, tilted camera, realistic photography angle, poster composition, pure 90-degree top-down view, aerial photography, realistic architectural photography, excessive depth perspective, blurry, low quality, messy layout
```
