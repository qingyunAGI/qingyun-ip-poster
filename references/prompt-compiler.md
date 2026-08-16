# 图像层与排版层指令编译

## 编译原则

为每个方向分别编写两份规范：

1. `art_prompt`：只描述主体、场景、镜头、光线、材质、留白和比例。
2. `layout_spec`：准确列出中文、姓名、身份、日期、Logo、断行、字号层级与对齐。

默认在 `art_prompt` 末尾加入：

```text
base artwork only, no readable text, no logo, no watermark,
preserve the specified clean text-safe zones
```

只有在当前图像工具能够可靠生成目标文字且最终会逐字校对时，才把文字交给模型直接渲染。

## 现实人物身份锁定块

```text
All supplied portrait references show the same real person: [姓名].
Use [最清晰正脸] as the primary identity anchor and use the remaining images
only for body proportions, pose, clothing and professional context.
Preserve facial shape, eye spacing, eyebrows, nose, mouth, jawline, hairline,
skin tone, age and distinctive features. Do not beautify into another person.
```

不依据姓名生成现实人物；没有授权照片时只做无脸剪影或等待用户补充。

## 商务个人 IP 底图模板

```text
3:4 vertical premium business editorial portrait poster base,
[现实人物身份锁定块],
[超近景/近景/半身/3/4身], subject placed [左/中/右],
[正面直视/侧面思考/演讲手势/双手交叠],
[服装与必须保留的配饰],
[峰会暗场/暖白编辑空间/石墨灰棚拍/会议桌/建筑空间],
controlled cinematic portrait lighting, realistic skin texture,
one clear visual center, restrained international magazine aesthetic,
clean safe zone at [标题区], secondary safe zone at [身份区],
5 to 6 percent outer margins, 3:4 vertical,
base artwork only, no readable text, no logo, no watermark
```

排版层：

```text
主标题：[原样文字]
语义断行：[第1行] / [第2行] / [第3行]
唯一强调：[关键词或数字]，颜色 [色值]
姓名：[原样文字]
身份：[原样文字]
背书：最多 5 条，仅用已核实内容
字体：主标题 [粗黑/窄黑/编辑宋体]；信息 [中性无衬线]
```

## Keynote 观点宣言底图模板

```text
3:4 vertical editorial keynote manifesto poster base,
[现实人物身份锁定块],
a realistic speaker centered or slightly offset, chest-up or half-body,
holding a supplied microphone or presentation clicker when present in the reference,
dark navy-black editorial background,
large low-contrast abstract condensed typographic slabs behind the person,
the subject layered in front of the background letterforms,
subtle warm orange rim light, very sparse ember particles,
natural skin texture, refined magazine-cover lighting,
clean top zone for series metadata,
calm lower-third safe zone for a large Chinese statement,
6 percent outer margins, high contrast but restrained,
base artwork only, no readable text, no logo, no watermark
```

排版层：

- 把观点控制在 14—24 个汉字、2—3 行。
- 把 2—5 字结论短语设为唯一强调色。
- 让补充句字号约为主观点的 18%—25%。
- 让姓名与身份保持第二/第三层级，不做第二个超大标题。

## 嘉宾观点卡底图模板

```text
3:4 vertical premium editorial speaker portrait,
[现实人物身份锁定块],
half-body studio portrait placed on the left 52 percent of the canvas,
face positioned in the upper-left quadrant,
direct gaze or inward gaze toward the empty text area,
deep seamless black background,
soft cinematic key light and subtle warm rim light,
natural realistic skin texture,
clear separation between dark clothing and background,
right 44 percent kept clean and low-detail for a large Chinese statement,
bottom-left safe zone for name and two-line role,
bottom full-width safe zone for a fixed event footer,
minimal, confident, serious editorial campaign aesthetic,
base artwork only, no readable text, no logo, no watermark
```

系列排版层：

```text
固定：网格、字体、标题起点、眼线、姓名基线、身份行高、页脚
变量：人物、18—30 字观点、2—5 字强调短语、一个强调色
活动事实：全部从同一份已核实事实表取值
```

## 9:16 活动总海报底图模板

```text
9:16 vertical high-impact editorial event campaign background,
a dark monumental stage built from massive metallic geometric slabs
derived from [活动缩写/品牌结构],
a vivid [强调色] circular backlight at the center,
six to eight professional silhouettes seated around a glossy round table,
cinematic symmetrical meeting scene,
strong black negative space, metallic silver structures framing the people,
subtle colored reflections on the table,
top-left safe zone for a large event title,
top-right safe zone for date and an authorized logo,
lower 28 percent kept dark and quiet for an editable guest lineup grid,
bottom safe zone for time and livestream call-to-action,
premium editorial campaign, dramatic but controlled,
realistic light and coherent perspective,
base artwork only, no readable text, no logo, no watermark
```

排版层按唯一活动事实表填充：

```text
活动主题：[原样文字]
日期：[YYYY-MM-DD]
时间：[HH:MM-HH:MM + 时区]
地点/平台：[原样文字]
嘉宾顺序：[固定顺序]
嘉宾身份：[每人最多 2 条]
CTA：[原样文字]
Logo：[使用用户提供的原文件，不生成]
```

巨型 `AI` 只用于 AI 主题；其他项目换成活动缩写、抽象建筑或品牌符号。需要准确字母时，后期用可编辑矢量/3D 字完成。

## 赛博修仙高键角色档案底图模板

```text
[角色身份与气质],
a cyber-xianxia character portrait combining refined Chinese cultivation aesthetics
with precision futuristic armor,
[锁定的脸、银发、发冠、首饰、武器和法器],
blackened silver armor with restrained dark-red lacquer details,
intricate chains and engraved mechanical components,
subtle iridescent translucent fabric,
three-quarter close-up, character placed on the right,
direct controlled gaze,
a weapon entering from the lower-left foreground with strong foreshortening,
face and eyes tack sharp, foreground weapon slightly out of focus,
high-key pearl-white studio background,
soft overcast key light and crisp silver rim light,
luxury game character dossier aesthetic,
clean editorial negative space on upper-left, mid-left and lower-left,
3:4 vertical, ultra-detailed realistic materials, cinematic but restrained,
base artwork only, no readable text, no logo, no watermark
```

排版层使用三类字体：宽体切角系列字标、高对比宋体/明朝体角色名、中性无衬线档案信息。红色面积控制在 3%—7%。

## 赛博修仙低键世界观底图模板

```text
[同一角色的身份与压迫感],
a dark cyber-xianxia warrior centered in a ceremonial frontal pose,
[与白版完全一致的脸、发型、服装结构、武器和饰件],
intricate blackened silver exoskeleton armor,
engraved cultivation motifs fused with precision machinery,
hands holding [符纸/法器] on the central axis,
a sheathed blade rising diagonally behind the shoulder,
controlled direct gaze,
symmetrical shoulder silhouette with one intentional diagonal break,
deep charcoal-black environment,
ghostlike ink-smoke forms and distant ancient architecture,
subtle mythic creature silhouette embedded in the darkness,
low-key cinematic lighting, cold silver rim light,
restrained blood-red accents and one small warm paper-toned focal point,
premium dark game key art, collectible edition cover,
clear top-left logo zone, narrow information zones on both sides,
clean footer zone, 3:4 vertical, deep blacks with preserved detail,
base artwork only, no readable text, no logo, no watermark
```

## 通用负面约束

```text
no fake readable Chinese or English, no random logo, no watermark,
no altered real-person identity, no celebrity invented from a name,
no plastic skin, no beauty-filter face, no malformed hands,
no duplicated limbs, no broken microphone, sword, chain or armor geometry,
no crowded interface, no cheap course-sales or livestream layout,
no rainbow neon, no excessive HUD, sparks, lens flare or glowing borders,
no unrelated client, award, event, brand or institution,
no text covering eyes, nose, mouth or required visual evidence
```

赛博修仙追加：

```text
no generic western sci-fi armor, no medieval European plate armor,
no cosplay studio look, no flat anime cel shading,
no oversaturated red, no iridescent rainbow plastic,
no random Chinese ornaments without structural purpose
```
