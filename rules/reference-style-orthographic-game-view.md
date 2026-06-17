# 参考图改风格 + 固定正交斜俯视游戏视角 Prompt 规范

这份规范用于后续处理“上传参考图，参考图内容不变，只改变画面风格，并固定传统正交斜俯视游戏视角”的任务。后续当用户发图并要求分析、改风格或迭代测试结果时，应优先参考本规范。

## 一、核心目标

当用户提供一张参考图时，AI 绘图需要做到：

1. 保留参考图的场景内容和空间布局。
2. 保留参考图的传统游戏正交斜俯视视角。
3. 只改变画面风格、材质、色彩、氛围和美术表现。
4. 不要把视角改成电影镜头、平视、低角度、广角透视或纯航拍顶视图。

## 二、视角固定的标准描述

### 中文标准描述

使用传统 2D 游戏地图视角，固定正交斜俯视镜头，三分之四俯视角，相机从上方向下约 45 度观察。画面采用正交投影 / 平行投影，不使用透视投影。地面是主要画面区域，建筑和物体应显示顶部，同时露出少量前立面和侧立面。整体像经典 JRPG / 手游村庄地图，空间清晰、可读性强、没有明显近大远小。

### 英文标准描述

Use a traditional 2D game map camera, fixed orthographic oblique top-down view, 3/4 top-down angle, camera looking downward at about 45 degrees. Use orthographic projection / parallel projection, not perspective projection. The ground plane should dominate the image. Buildings and objects should show their top surfaces with slight front and side facades visible. The scene should feel like a classic JRPG / mobile game village map, highly readable, with no obvious perspective scaling.

## 三、参考图约束描述

### 中文写法

严格参考上传图片中的场景结构、空间布局、建筑位置、道路走向、水面位置、角色与道具的大致分布。保持原图的地图式构图和俯视游戏镜头，不改变主要物体之间的位置关系。只改变美术风格、细节设计、色彩气氛和材质表现。

### 英文写法

Strictly follow the reference image for scene structure, spatial layout, building placement, road direction, water placement, and the general distribution of characters and props. Preserve the map-like composition and top-down game camera from the reference. Do not change the main spatial relationships between objects. Only change the art style, detail design, color mood, and material rendering.

## 四、风格替换描述模板

### 中文模板

```text
将参考图中的场景改造成【目标风格】。保留原图的场景内容、构图、建筑位置、道路、水面、道具分布和传统正交斜俯视游戏视角。画面风格变为【具体风格关键词】，色彩倾向【色彩关键词】，氛围为【氛围关键词】，材质表现为【材质关键词】。整体应像一张高完成度的 2D 游戏场景地图，而不是电影截图或插画海报。
```

### 英文模板

```text
Transform the reference scene into 【target style】. Preserve the original scene content, composition, building placement, roads, water areas, prop distribution, and traditional orthographic oblique top-down game camera. The art style should become 【style keywords】, with 【color keywords】 colors, 【mood keywords】 atmosphere, and 【material keywords】 material rendering. The final image should look like a polished 2D game environment map, not a cinematic screenshot or poster illustration.
```

## 五、完整通用 Prompt 模板

### 中文版

```text
参考上传图片，保留原图中的场景结构、空间布局、建筑位置、道路走向、水面区域、角色和道具的大致分布。保持原图的传统 2D 游戏地图视角：固定正交斜俯视镜头，三分之四俯视角，相机从上方向下约 45 度观察，使用正交投影 / 平行投影，不使用透视投影。地面占主要画面，建筑显示屋顶，并露出少量前立面和侧立面，整体像经典 JRPG / 手游村庄地图，空间清晰、可读性强。

将画面风格改为【目标风格】。使用【色彩关键词】色调，营造【氛围关键词】氛围。材质表现为【材质关键词】，细节精致但不要破坏原图的地图布局。整体是高完成度 2D 手绘游戏场景背景，画面干净、层次清楚、道具分布自然。

禁止改变视角，禁止平视，禁止低角度，禁止仰视，禁止电影镜头，禁止广角畸变，禁止鱼眼，禁止强透视，禁止明显近大远小，禁止纯 90 度顶视图，禁止把场景改成海报式构图。
```

### 英文版

```text
Use the uploaded image as the reference. Preserve the original scene structure, spatial layout, building placement, road direction, water areas, and the general distribution of characters and props. Keep the original traditional 2D game map camera: fixed orthographic oblique top-down view, 3/4 top-down angle, camera looking downward at about 45 degrees, using orthographic projection / parallel projection, not perspective projection. The ground plane should dominate the image. Buildings should show their rooftops with slight front and side facades visible. The whole scene should feel like a classic JRPG / mobile game village map, clear and highly readable.

Transform the visual style into 【target style】. Use a 【color keywords】 color palette and create a 【mood keywords】 atmosphere. Materials should feel like 【material keywords】, with refined details while preserving the original map layout. The final image should be a polished 2D hand-painted game environment background, clean, layered, and naturally arranged.

Do not change the camera angle. No eye-level view, no low angle, no worm’s-eye view, no cinematic camera, no wide-angle distortion, no fisheye, no strong perspective, no obvious near-far scaling, no pure 90-degree top-down view, and no poster-like composition.
```

## 六、视角关键词库

### 中文关键词

- 传统 2D 游戏地图视角
- 正交斜俯视
- 固定俯视镜头
- 三分之四俯视角
- 平行投影
- 正交投影
- 无透视变形
- 无灭点透视
- 地图式构图
- 经典 JRPG 村庄地图
- 手游地图场景
- 地面为主
- 屋顶可见
- 少量建筑立面可见
- 高可读性场景布局

### 英文关键词

- traditional 2D game map camera
- orthographic oblique top-down view
- fixed overhead RPG camera
- 3/4 top-down angle
- parallel projection
- orthographic projection
- no perspective distortion
- no vanishing point perspective
- map-like composition
- classic JRPG village map
- mobile game environment
- ground-dominant composition
- visible rooftops
- slight building facades visible
- highly readable environment layout

## 七、负面提示词库

### 中文负面提示词

- 平视
- 低角度
- 仰视
- 电影镜头
- 广角镜头
- 鱼眼镜头
- 强透视
- 灭点透视
- 近大远小
- 动态倾斜镜头
- 真实摄影感
- 海报构图
- 纯 90 度顶视图
- 航拍照片
- 写实建筑摄影
- 过度纵深感

### 英文负面提示词

- eye-level view
- low angle
- worm’s-eye view
- cinematic camera
- wide-angle lens
- fisheye lens
- strong perspective
- vanishing point perspective
- obvious perspective scaling
- tilted camera
- realistic photography angle
- poster composition
- pure 90-degree top-down view
- aerial photography
- realistic architectural photography
- excessive depth perspective

## 八、常用风格替换关键词

### 1. 治愈日系幻想手游风

中文关键词：2D 手绘游戏场景，日系幻想，治愈田园，童话村庄，低饱和蓝绿色调，柔和赛璐璐阴影，Q 版冒险感，绘本质感，温馨生活模拟，精致小物件堆叠。

英文关键词：2D hand-painted game scene, Japanese fantasy mobile game style, cozy fantasy village, healing countryside, low-saturation blue-green palette, soft cel shading, cute adventure feeling, storybook texture, warm life simulation, detailed small props.

### 2. 韩漫奇幻 RPG 场景风

中文关键词：韩漫式奇幻场景，高完成度 2D 背景，干净线条，柔和光影，精致建筑细节，梦幻色彩，清晰层次，轻幻想村庄，漫画感材质，细腻氛围。

英文关键词：Korean webtoon fantasy environment, polished 2D background, clean linework, soft lighting, refined architectural details, dreamy colors, clear layering, light fantasy village, comic-style materials, delicate atmosphere.

### 3. 暗黑奇幻村庄风

中文关键词：暗黑奇幻村庄，低明度色彩，冷色月光，潮湿石板路，古旧木屋，神秘森林，微弱灯火，阴影层次，哥特童话感，压抑但精致。

英文关键词：dark fantasy village, low-key color palette, cold moonlight, wet stone paths, old wooden houses, mysterious forest, faint warm lights, layered shadows, gothic fairytale mood, gloomy but refined.

### 4. 蒸汽朋克小镇风

中文关键词：蒸汽朋克村庄，铜管机械，齿轮装饰，烟囱蒸汽，复古工业建筑，暖棕色调，复杂道具，手绘游戏背景，奇幻机械小镇。

英文关键词：steampunk village, brass pipes, gear decorations, chimney steam, retro industrial buildings, warm brown palette, complex props, hand-painted game background, fantasy mechanical town.

### 5. 废土末日营地风

中文关键词：废土营地，破旧建筑，临时棚屋，锈蚀金属，杂乱道具，灰黄低饱和色调，末日生存感，荒草石块，破损道路，手绘游戏地图。

英文关键词：post-apocalyptic camp, ruined buildings, temporary shelters, rusty metal, scattered props, gray-yellow low-saturation palette, survival atmosphere, wild grass and rocks, broken roads, hand-painted game map.

## 九、测试用 Prompt 示例

### 示例 1：把参考图改成治愈日系幻想村庄

```text
参考上传图片，保留原图中的场景结构、空间布局、建筑位置、道路走向、水面区域、角色和道具的大致分布。保持原图的传统 2D 游戏地图视角：固定正交斜俯视镜头，三分之四俯视角，相机从上方向下约 45 度观察，使用正交投影 / 平行投影，不使用透视投影。地面占主要画面，建筑显示屋顶，并露出少量前立面和侧立面，整体像经典 JRPG / 手游村庄地图，空间清晰、可读性强。

将画面风格改为治愈日系幻想手游风格，2D 手绘游戏场景，童话村庄，温馨生活模拟氛围，低饱和蓝绿色调，柔和赛璐璐阴影，绘本质感，精致小物件堆叠。画面干净、柔和、梦幻，有清晨或夜晨交界的安静氛围。

禁止改变视角，禁止平视，禁止低角度，禁止电影镜头，禁止广角畸变，禁止鱼眼，禁止强透视，禁止明显近大远小，禁止纯 90 度顶视图，禁止把场景改成海报式构图。
```

### 示例 2：把参考图改成韩漫奇幻 RPG 村庄

```text
参考上传图片，严格保留原图的村庄地图布局、建筑分布、道路、水面、树木、石块和道具位置关系。保持传统正交斜俯视游戏视角，固定三分之四俯视角，正交投影，平行投影，无透视变形，无灭点透视。地面为主，建筑屋顶清晰可见，同时露出少量前立面和侧立面，像经典 RPG 手游地图。

将场景改为韩漫奇幻 RPG 场景风格，高完成度 2D 手绘背景，干净精致线条，柔和光影，细腻建筑细节，梦幻色彩，轻幻想村庄氛围。保留游戏场景的可读性和地图式布局，不要变成电影分镜或人物海报。

负面提示词：平视，低角度，仰视，电影镜头，广角，鱼眼，强透视，灭点透视，近大远小，真实摄影，海报构图，纯顶视图。
```

### 示例 3：把参考图改成暗黑奇幻村庄

```text
参考上传图片，保持原图的场景内容、空间布局、道路走向、水面位置、建筑和道具分布。视角必须保持为传统 2D 游戏地图视角，固定正交斜俯视，三分之四俯视角，相机从上方向下约 45 度，正交投影 / 平行投影，无透视畸变。地面占主要画面，屋顶和少量建筑立面同时可见，整体是清晰可读的 RPG 地图场景。

将画面改成暗黑奇幻村庄风格，低明度色彩，冷色月光，潮湿石板路，古旧木屋，神秘森林，微弱灯火，阴影层次丰富，哥特童话感，压抑但精致。保留原图地图布局，只改变美术风格和氛围。

禁止平视、低角度、仰视、电影镜头、强透视、广角畸变、鱼眼、航拍照片、纯 90 度顶视图、真实建筑摄影感。
```

## 十、最推荐的最终写法结构

以后写 Prompt 时，建议按照这个顺序：

1. 先说参考图约束：保留参考图内容、布局、物体位置关系。
2. 再锁定视角：正交斜俯视、三分之四俯视、平行投影、无透视。
3. 再写目标风格：韩漫、日系、暗黑、蒸汽朋克、废土等。
4. 再写色彩和氛围：低饱和、冷色月光、暖色灯光、梦幻、压抑、治愈等。
5. 最后写负面提示词：禁止平视、低角度、广角、强透视、电影镜头等。

## 十一、一句话极简版

参考图内容和布局不变，只改变美术风格；保持传统 2D 游戏地图视角，固定正交斜俯视，三分之四俯视角，正交 / 平行投影，无透视变形，地面为主，屋顶和少量建筑立面可见，像经典 JRPG 手游村庄地图；禁止平视、低角度、电影镜头、广角、鱼眼、强透视和纯顶视图。
