# Qingyun IP Poster · 中文说明

<p align="center"><code>$qingyun-ip-poster</code></p>

<p align="center">
  <strong>把零散素材编译成一套有主张、有识别、能持续发布的视觉系统。</strong>
</p>

<p align="center">
  <a href="README.md">视觉首页</a> ·
  <a href="README.en.md">English</a> ·
  <a href="#安装">安装</a> ·
  <a href="https://github.com/qingyunAGI/qingyun-ip-poster/releases/latest">最新版本</a>
</p>

<table>
  <tr>
    <td width="33.33%"><img src="assets/style-references/04-high-contrast-closeup.png" alt="商务个人 IP 近景海报"></td>
    <td width="33.33%"><img src="assets/style-references/08-cyber-xianxia-worldview-keyart-dark.png" alt="创意角色世界观海报"></td>
    <td width="33.33%"><img src="assets/style-references/10-event-lineup-monumental.png" alt="多人活动总海报"></td>
  </tr>
</table>

## 安装

Windows PowerShell：

```powershell
git clone https://github.com/qingyunAGI/qingyun-ip-poster.git "$env:USERPROFILE\.codex\skills\qingyun-ip-poster"
```

macOS / Linux：

```bash
git clone https://github.com/qingyunAGI/qingyun-ip-poster.git ~/.codex/skills/qingyun-ip-poster
```

安装后重启 Codex 或重新加载 Skills：

```text
$qingyun-ip-poster
```

更新现有版本：

```powershell
git -C "$env:USERPROFILE\.codex\skills\qingyun-ip-poster" pull
```

不使用 Git 时，可从 [Releases](https://github.com/qingyunAGI/qingyun-ip-poster/releases/latest) 下载 ZIP。

## 真实案例：改变的不是滤镜，而是视觉秩序

王磊把 Skill 用进真实账号后反馈：**“用上了。”**

<table>
  <tr>
    <th width="38%">使用前</th>
    <th width="24%">视觉 DNA</th>
    <th width="38%">使用 Skill 后</th>
  </tr>
  <tr>
    <td><img src="assets/case-studies/wang-lei-before-account-grid.jpg" alt="王磊使用 Skill 前的账号九宫格"></td>
    <td align="center" valign="middle">
      人物锚点<br><br>
      标题层级<br><br>
      字体与网格<br><br>
      姓名区与页脚<br><br>
      缩略图识别
    </td>
    <td><img src="assets/case-studies/wang-lei-after-account-grid.jpg" alt="王磊使用 Skill 后的账号九宫格"></td>
  </tr>
</table>

可观察的变化：先看到人物与主张，再读身份和细节；单张封面成立，九宫格并排时也有稳定的栏目感。

> 证据边界：两组截图不是同题材、同文案、同发布时间的严格 A/B 测试，只用于比较视觉秩序，不据此推断流量、点击或转化。

### 王磊商务个人 IP 五套表达

<table>
  <tr>
    <td width="50%" rowspan="2"><img src="assets/style-references/04-high-contrast-closeup.png" alt="王磊高对比近景观点海报"></td>
    <td width="25%"><img src="assets/style-references/01-black-neon-green.png" alt="王磊黑底荧光绿峰会海报"></td>
    <td width="25%"><img src="assets/style-references/02-ivory-editorial.png" alt="王磊象牙白编辑风海报"></td>
  </tr>
  <tr>
    <td><img src="assets/style-references/03-graphite-thought-leader.png" alt="王磊石墨灰思想领袖海报"></td>
    <td><img src="assets/style-references/05-black-gold-authority.png" alt="王磊黑金权威感海报"></td>
  </tr>
</table>

五套方案共享人物身份、字体秩序与品牌气质，但在景别、位置、动作、场景、标题结构和信息密度上真实变化。

## 四种任务路由

| 模式 | 默认交付 | 需要什么 | 比例 |
| --- | --- | --- | --- |
| 商务个人 IP 批量 | 账号视觉诊断 + 7 个差异方向，选 1—3 张精修 | 现有九宫格（可选）+ 3—5 张人物照 + 观点/履历 | 3:4 |
| Keynote 观点宣言 | 3 个方向或指定 1 张 | 演讲/半身照 + 一句可核实观点 | 3:4 |
| 嘉宾与活动整套 | 1 张活动总海报 + N 张嘉宾卡 | 活动事实表 + Logo + 嘉宾资料/照片 | 9:16 + 3:4 |
| 创意 IP 角色主视觉 | 高键角色档案 + 低键世界观 Key Art | 角色参考图或角色/世界观简报 | 3:4 |

任务路由先决定素材、比例、网格、版本数量和质量门槛。活动整套按实际嘉宾数生成，不强行套入 5/7/10 张逻辑。

## Visual System Edition 如何工作

1. **审计现状**：有账号截图时，先检查人物锚点、标题层级、系列秩序和缩略图可读性。
2. **建立事实卡**：区分用户提供、已核实和待核实内容，不补写奖项、客户或身份。
3. **定义视觉 DNA**：确定字体、网格、人物尺度、色彩、标题区、姓名区和页脚。
4. **规划真实差异**：用 2—3 个版式家族与近景、半身、环境三档尺度建立连续变化。
5. **分离图文两层**：模型负责人物、场景、光线、材质和留白；准确中文、Logo、日期后期排版。
6. **双重验收**：既检查单张海报，也检查整组九宫格和平台裁切。

## 三类扩展视觉

<table>
  <tr>
    <th width="33.33%">角色世界观</th>
    <th width="33.33%">Keynote 观点</th>
    <th width="33.33%">活动传播</th>
  </tr>
  <tr>
    <td><img src="assets/style-references/06-cyber-xianxia-character-dossier-light.png" alt="高键角色档案海报"></td>
    <td><img src="assets/style-references/07-keynote-manifesto-dark.png" alt="Keynote 观点宣言海报"></td>
    <td><img src="assets/style-references/10-event-lineup-monumental.png" alt="九比十六活动总海报"></td>
  </tr>
</table>

完整范式库包含 [12 张用户提供的原始样本](assets/style-references/)。它们用于提取构图、层级、材质和系列规则，不是可直接复用的事实模板。

## 直接说人话就能用

```text
$qingyun-ip-poster
这是我现在的账号九宫格和 5 张人物照片。先诊断视觉问题，
再建立一套可以连续发布的视觉 DNA，并做 7 张构图真实不同的 3:4 海报。
```

```text
$qingyun-ip-poster
把这场圆桌活动做成 1 张 9:16 总海报和 6 张 3:4 嘉宾观点卡。
日期、时间、姓名、身份和 Logo 只使用我提供的事实表。
```

```text
$qingyun-ip-poster
基于这张角色设定图，做高键白角色档案和低键黑世界观 Key Art。
锁定脸、发型、服装、武器和饰件，不要霓虹城市和满屏 HUD。
```

## 交付红线

以下问题未修复时，不交付：

- 人脸不像本人，或同一角色在不同版本中漂移。
- 中文、姓名、身份、日期、时间或 Logo 错误。
- 出现用户未提供的奖项、客户、活动、品牌或现实人物身份。
- 手、麦克风、武器、盔甲、桌椅或人体比例畸形。
- 重要信息落入平台裁切或操作区。
- 缩略图无法识别人物和核心主张。
- 同批作品只是换色，没有真实构图差异。
- 把非同题材的前后截图包装成流量或转化 A/B 测试。

## 目录结构

```text
qingyun-ip-poster/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   ├── case-studies/           # 真实账号前后对比证据
│   └── style-references/       # 12 张原始参考海报
├── references/
│   ├── design-system.md
│   ├── failure-modes.md
│   ├── intake-guide.md
│   ├── prompt-compiler.md
│   ├── quality-checklist.md
│   └── version-matrix.md
├── README.md                    # 中文视觉首页
├── README.zh-CN.md              # 完整中文说明
└── README.en.md                 # English documentation
```

## 作者与商务合作

**彭青云（Kaiwen）**持续实践 AI 视频、个人 IP、视觉叙事与可复用创作工作流，并把高频方法沉淀为 Codex Skills、提示词与课程资产。

GitHub：[@qingyunAGI](https://github.com/qingyunAGI)

需要定制个人账号、课程、活动或团队视觉系统，可通过 [GitHub Issue](https://github.com/qingyunAGI/qingyun-ip-poster/issues/new) 提交公开需求；敏感原图和未公开商业信息请勿上传到公开 Issue。

---

当前版本：**1.2.0 Visual System Edition**。仓库暂未附带开放许可证；转载、二次分发或商业打包前请联系作者。
