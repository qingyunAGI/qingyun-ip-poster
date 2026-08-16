# Qingyun IP Poster

<p align="center">
  <strong>一个 Skill，完成商务个人 IP、Keynote 观点、嘉宾活动整套与创意角色主视觉。</strong>
</p>

<p align="center">
  <code>$qingyun-ip-poster</code>
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="#一键安装">一键安装</a> ·
  <a href="https://github.com/qingyunAGI/qingyun-ip-poster/releases/latest">最新版本</a>
</p>

<p align="center">
  <img alt="版本 1.1.0" src="https://img.shields.io/badge/version-1.1.0-C8A66A">
  <img alt="Codex Skill" src="https://img.shields.io/badge/Codex-Skill-111111">
  <img alt="海报比例 3:4 与 9:16" src="https://img.shields.io/badge/poster-3%3A4%20%7C%209%3A16-4B5D36">
  <img alt="12 张参考海报" src="https://img.shields.io/badge/style%20references-12-8138EE">
</p>

## v1.1 新增设计系统

### 赛博修仙：高键角色档案 × 低键世界观 Key Art

<p align="center">
  <img src="assets/style-references/06-cyber-xianxia-character-dossier-light.png" width="46%" alt="赛博修仙高键白角色档案海报">
  <img src="assets/style-references/08-cyber-xianxia-worldview-keyart-dark.png" width="46%" alt="赛博修仙低键黑世界观海报">
</p>

### Keynote 观点 × 嘉宾系列卡

<p align="center">
  <img src="assets/style-references/07-keynote-manifesto-dark.png" width="31%" alt="暗场 Keynote 观点宣言海报">
  <img src="assets/style-references/09-guest-manifesto-orange-cap.png" width="31%" alt="橙色嘉宾观点卡">
  <img src="assets/style-references/12-guest-manifesto-purple.png" width="31%" alt="紫色嘉宾观点卡">
</p>

### 9:16 活动总海报 × 单人嘉宾衍生卡

<p align="center">
  <img src="assets/style-references/10-event-lineup-monumental.png" width="36%" alt="巨字舞台式多人活动总海报">
  <img src="assets/style-references/11-guest-manifesto-orange-suit.png" width="48%" alt="单人嘉宾观点卡">
</p>

完整参考库还保留 5 张原有商务个人 IP 母版，共计 [12 张用户提供的原始样本](assets/style-references/)。图片内嵌的姓名、身份、奖项、日期、Logo、版本号与角色文案未在本仓库复核真实性，只作为版式参考；不得摘引为事实或自动带入新作品，使用者还需自行确认肖像与品牌授权。

其中活动总海报保留原始 `941 × 1672` 尺寸，接近 9:16；正式生产统一输出精确的 `1080 × 1920` 或其他等比 9:16 尺寸。样本中出现的 `V1.0.0` 属于画面内的示例文案，不代表当前 Skill 版本。

## 一键安装

Windows PowerShell：

```powershell
git clone https://github.com/qingyunAGI/qingyun-ip-poster.git "$env:USERPROFILE\.codex\skills\qingyun-ip-poster"
```

macOS / Linux：

```bash
git clone https://github.com/qingyunAGI/qingyun-ip-poster.git ~/.codex/skills/qingyun-ip-poster
```

安装后重启 Codex 或重新加载 Skills，直接调用：

```text
$qingyun-ip-poster
```

更新已安装版本：

```powershell
git -C "$env:USERPROFILE\.codex\skills\qingyun-ip-poster" pull
```

如果不使用 Git，也可以从 [GitHub Releases](https://github.com/qingyunAGI/qingyun-ip-poster/releases/latest) 下载最新版 ZIP。

## 四种任务路由

| 模式 | 默认交付 | 需要什么 | 比例 |
| --- | --- | --- | --- |
| 商务个人 IP 批量 | 7 个差异方向，选 1—3 张精修 | 3—5 张同一人物照片 + 观点/履历 | 3:4 |
| Keynote 观点宣言 | 3 个方向或指定 1 张 | 演讲/半身照 + 一句观点 | 3:4 |
| 嘉宾与活动整套 | 1 张活动总海报 + N 张嘉宾卡 | 活动事实表 + Logo + 嘉宾资料/照片 | 9:16 + 3:4 |
| 创意 IP 角色主视觉 | 高键白 + 低键黑双版本 | 角色参考图或角色/世界观简报 | 3:4 |

这次升级不只是增加案例图，而是改变了 Skill 的判断方式：先路由任务，再选择素材、比例、网格、生成数量和质量门槛。活动整套按真实嘉宾数生成，不再强行套入 5/7/10 张逻辑。

## 核心原则

- **信息第一**：远看先识别主张、人物/角色或活动主题，近看再读身份与细节。
- **身份准确**：现实人物使用照片作为身份锚点；不能只按姓名生成现实人物。
- **事实准确**：姓名、职位、奖项、数字、日期、Logo 和引语必须来自用户材料或可追溯来源。
- **图文分层**：模型生成主体、场景、光线、材质与留白；关键中文、Logo 和日期用可控排版完成。
- **系列统一**：统一字体、网格、人物尺度、光比和页脚；差异来自镜头、动作、场景和叙事。
- **单一强调**：一张海报只使用一个视觉中心、一个强调短语和一种高饱和强调色。

## 使用流程

1. **任务路由**：判断是个人 IP、Keynote、活动整套还是角色主视觉。
2. **事实编译**：建立唯一信息卡，标记用户提供、已核实和待核实内容。
3. **范式选择**：从 12 张样本提取构图、网格、材质与层级，不复制样本文案。
4. **图像生产**：生成主体、场景、光线和清晰文字安全区。
5. **准确排版**：放入中文、姓名、日期、Logo、嘉宾矩阵和页脚。
6. **逐张质检**：检查身份、角色连续性、事实、中文、肢体、器物、缩略图和平台裁切。
7. **筛选精修**：推荐最值得继续优化的 1—3 个方向。

## 示例调用

```text
$qingyun-ip-poster
用这 4 张人物照做 7 张 3:4 个人 IP 海报。标题和履历必须原样保留，
每张在镜头、人物位置、场景和标题结构上明显不同。
```

```text
$qingyun-ip-poster
把这场圆桌活动做成 1 张 9:16 总海报和 6 张 3:4 嘉宾观点卡。
所有日期、时间、姓名、身份和 Logo 只使用我提供的事实表。
```

```text
$qingyun-ip-poster
基于这张角色设定图，做高键白角色档案和低键黑世界观 Key Art 双版本。
锁定脸、银发、发冠、机械甲、武器和暗朱红点睛，不要霓虹城市和满屏 HUD。
```

## 质量门槛

以下问题未修复时，不交付：

- 人脸不像本人，或同一角色在不同版本中漂移。
- 中文、姓名、身份、日期、时间或 Logo 错误。
- 出现用户未提供的奖项、客户、活动、品牌或现实人物身份。
- 手、麦克风、剑、链条、盔甲、桌椅或人体比例畸形。
- 重要信息落入平台裁切或操作区。
- 缩略图无法识别主体和核心主张。
- 同批海报只是换色，没有真实构图差异。

## 目录结构

```text
qingyun-ip-poster/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── style-references/       # 12 张原始参考海报
├── references/
│   ├── design-system.md
│   ├── failure-modes.md
│   ├── intake-guide.md
│   ├── prompt-compiler.md
│   ├── quality-checklist.md
│   └── version-matrix.md
├── README.md
└── README.zh-CN.md
```

## 作者

**彭青云（Kaiwen）**持续实践 AI 视频、个人 IP、视觉叙事与可复用创作工作流，并把高频生产方法沉淀为 Codex Skills、提示词与课程资产。

GitHub：[@qingyunAGI](https://github.com/qingyunAGI)

---

当前版本：**1.1.0**。仓库暂未附带开放许可证；转载、二次分发或商业打包前请联系作者。
