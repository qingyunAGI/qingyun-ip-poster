# Qingyun IP Poster

<p align="center"><code>$qingyun-ip-poster</code></p>

<p align="center">
  <strong>不是生成一张海报，而是建立一套能持续发布的视觉系统。</strong><br>
  <sub>从账号诊断、人物识别与观点编译，到 3:4 海报、9:16 活动总视觉和系列化交付。</sub>
</p>

<p align="center">
  <a href="README.zh-CN.md">完整中文说明</a> ·
  <a href="README.en.md">English</a> ·
  <a href="#30-秒开始">一键安装</a> ·
  <a href="https://github.com/qingyunAGI/qingyun-ip-poster/releases/latest">下载最新版</a>
</p>

<p align="center">
  <img alt="Version 1.2.0" src="https://img.shields.io/badge/version-1.2.0-C8A66A">
  <img alt="Visual system" src="https://img.shields.io/badge/output-visual%20system-111111">
  <img alt="Poster ratios" src="https://img.shields.io/badge/poster-3%3A4%20%7C%209%3A16-4B5D36">
  <img alt="12 references" src="https://img.shields.io/badge/style%20references-12-8138EE">
</p>

<table>
  <tr>
    <td width="33.33%"><img src="assets/style-references/04-high-contrast-closeup.png" alt="商务个人 IP 强识别近景海报"></td>
    <td width="33.33%"><img src="assets/style-references/06-cyber-xianxia-character-dossier-light.png" alt="赛博修仙高键角色档案海报"></td>
    <td width="33.33%"><img src="assets/style-references/10-event-lineup-monumental.png" alt="九比十六多人活动总海报"></td>
  </tr>
  <tr>
    <th>商务个人 IP</th>
    <th>创意角色 Key Art</th>
    <th>活动整套视觉</th>
  </tr>
</table>

## 30 秒开始

Windows PowerShell，一行复制：

```powershell
git clone https://github.com/qingyunAGI/qingyun-ip-poster.git "$env:USERPROFILE\.codex\skills\qingyun-ip-poster"
```

安装后重启 Codex 或重新加载 Skills，直接说：

```text
$qingyun-ip-poster
这是我的账号九宫格、5 张人物照和本期观点。先诊断现有视觉，再做一套可以连续发布的海报。
```

<details>
<summary><strong>macOS / Linux 安装与现有版本更新</strong></summary>

```bash
git clone https://github.com/qingyunAGI/qingyun-ip-poster.git ~/.codex/skills/qingyun-ip-poster
```

```powershell
git -C "$env:USERPROFILE\.codex\skills\qingyun-ip-poster" pull
```

</details>

## 从零散封面，到有记忆的账号

王磊把 Skill 放进真实发布流程后，只回复了三个字：**“用上了。”**

<table>
  <tr>
    <th width="38%">使用前</th>
    <th width="24%">改变的不是滤镜</th>
    <th width="38%">使用 Skill 后</th>
  </tr>
  <tr>
    <td><img src="assets/case-studies/wang-lei-before-account-grid.jpg" alt="王磊使用 Skill 前的账号封面九宫格"></td>
    <td align="center" valign="middle">
      <strong>人物成为锚点</strong><br><br>
      标题先于履历<br><br>
      网格与页脚稳定<br><br>
      缩略图仍能识别<br><br>
      <strong>单张 → 系统</strong>
    </td>
    <td><img src="assets/case-studies/wang-lei-after-account-grid.jpg" alt="王磊使用 Skill 后的账号封面九宫格"></td>
  </tr>
</table>

> 这不是同题材、同文案、同发布时间的流量 A/B 测试。它只证明视觉秩序发生了可观察的变化，不据此虚构点击或转化提升。

## 一个人，可以有五种表达；但仍然像同一个品牌

<table>
  <tr>
    <td width="50%" rowspan="2"><img src="assets/style-references/04-high-contrast-closeup.png" alt="王磊高对比近景观点海报"></td>
    <td width="25%"><img src="assets/style-references/01-black-neon-green.png" alt="王磊黑底荧光绿峰会海报"></td>
    <td width="25%"><img src="assets/style-references/02-ivory-editorial.png" alt="王磊象牙白编辑风顾问海报"></td>
  </tr>
  <tr>
    <td><img src="assets/style-references/03-graphite-thought-leader.png" alt="王磊石墨灰思想领袖海报"></td>
    <td><img src="assets/style-references/05-black-gold-authority.png" alt="王磊黑金权威感海报"></td>
  </tr>
</table>

统一的是人物身份、字体秩序、标题逻辑和品牌气质；变化的是景别、动作、场景、信息密度与叙事。**这不是一张模板换五次颜色。**

## 一套 Skill，覆盖三种高频传播任务

<table>
  <tr>
    <th width="33.33%">创意 IP</th>
    <th width="33.33%">观点传播</th>
    <th width="33.33%">活动整套</th>
  </tr>
  <tr>
    <td><img src="assets/style-references/08-cyber-xianxia-worldview-keyart-dark.png" alt="赛博修仙世界观主视觉"></td>
    <td><img src="assets/style-references/07-keynote-manifesto-dark.png" alt="Keynote 观点宣言海报"></td>
    <td><img src="assets/style-references/10-event-lineup-monumental.png" alt="多人圆桌活动总海报"></td>
  </tr>
  <tr>
    <td>角色档案 + 世界观 Key Art</td>
    <td>人物锚点 + 一句核心判断</td>
    <td>总海报 + N 张嘉宾衍生卡</td>
  </tr>
</table>

## 它真正替你做的五件事

| 不是 | 而是 |
| --- | --- |
| 看见参考图就模仿 | 先判断个人 IP、观点、活动或角色任务 |
| 把履历全部塞进画面 | 编译主张、身份、证据与信息优先级 |
| 一张人物照无限换背景 | 建立 2—3 个版式家族和真实构图差异 |
| 让模型碰运气写中文 | 分离图像层与准确排版层 |
| 交够数量就结束 | 检查身份、事实、肢体、文字、裁切与九宫格效果 |

## 商务落地

适合个人账号、课程、直播活动、峰会嘉宾、品牌栏目与创意 IP 验证。需要定制持续视觉系统，可通过 [GitHub Issue](https://github.com/qingyunAGI/qingyun-ip-poster/issues/new) 说明平台、数量、时间和现有视觉问题；敏感原图与未公开商业信息不要上传到公开 Issue。

案例方法与创作过程：[我把商用级高审美海报 Skill，开源了](https://mp.weixin.qq.com/s/NRuhMds4UYYwiZ-aJpjv0A)

---

作者：**彭青云（Kaiwen）** · GitHub [@qingyunAGI](https://github.com/qingyunAGI)

当前版本：**1.2.0 Visual System Edition**。仓库暂未附带开放许可证；转载、二次分发或商业打包前请联系作者。
