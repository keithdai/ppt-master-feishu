---
deck_id: feishu_lark_h5
kind: deck
category: scenario
summary: 飞书/Lark H5 风格深色客户提案模板，适用于售前方案、产品演示、AI 工作方式宣讲和高管汇报.
keywords: [feishu, lark, h5, proposal, dark, deckjson, customer-deck]
primary_color: "#3C7FFF"
canvas_format: ppt169
replication_mode: fidelity
placeholders:
  01_cover: ["{{TITLE}}", "{{SUBTITLE}}", "{{AUTHOR}}", "{{DATE}}"]
  02_agenda: ["{{PAGE_TITLE}}", "{{AGENDA_ITEM_1}}", "{{AGENDA_ITEM_2}}", "{{AGENDA_ITEM_3}}", "{{AGENDA_ITEM_4}}", "{{AGENDA_ITEM_5}}", "{{AGENDA_ITEM_6}}"]
  02_chapter: ["{{CHAPTER_NUM}}", "{{CHAPTER_TITLE}}", "{{CHAPTER_DESC}}"]
  03a_content_3up: ["{{PAGE_TITLE}}", "{{CARD_1_TITLE}}", "{{CARD_1_BODY}}", "{{CARD_2_TITLE}}", "{{CARD_2_BODY}}", "{{CARD_3_TITLE}}", "{{CARD_3_BODY}}"]
  03b_content_2col: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{FEATURE_1}}", "{{FEATURE_2}}", "{{FEATURE_3}}", "{{FEATURE_4}}", "{{VISUAL_TITLE}}"]
  03c_content_quote: ["{{PAGE_TITLE}}", "{{QUOTE_TEXT}}", "{{QUOTE_AUTHOR}}"]
  03d_content_stats: ["{{PAGE_TITLE}}", "{{KPI_1_NUM}}", "{{KPI_1_LABEL}}", "{{KPI_2_NUM}}", "{{KPI_2_LABEL}}", "{{KPI_3_NUM}}", "{{KPI_3_LABEL}}", "{{KPI_4_NUM}}", "{{KPI_4_LABEL}}"]
  03e_content_big_stat: ["{{EYEBROW}}", "{{BIG_NUMBER}}", "{{BIG_UNIT}}", "{{PAGE_TITLE}}", "{{KEY_MESSAGE}}"]
  03f_content_table: ["{{PAGE_TITLE}}", "{{CONTENT_AREA}}"]
  03g_content_timeline: ["{{PAGE_TITLE}}", "{{STEP_1}}", "{{STEP_2}}", "{{STEP_3}}", "{{STEP_4}}"]
  03h_content_logowall: ["{{PAGE_TITLE}}", "{{CONTENT_AREA}}"]
  04_ending: ["{{TITLE}}", "{{SUBTITLE}}", "{{CTA_TEXT}}"]
---

# 飞书 Lark H5 提案模板 — Design Specification

## I. Template Overview

飞书/Lark H5 客户提案风格，迁移自 `feishu-deck-h5` 的 DeckJSON 设计系统。整体采用深色全屏网页演示感，结合飞书官方背景资产、蓝紫青渐变 keyline、半透明信息卡片和严格字号阶梯，适合做可反复复用的售前、方案、AI 工作方式、数字化转型主题演示。

| 项目 | 设定 |
|---|---|
| 适用场景 | 客户提案、产品解决方案、AI 工作方式宣讲、高管汇报、销售内训 |
| 设计调性 | Feishu official, dark, structured, premium, SaaS proposal |
| 主题模式 | 全深色主题，封面/章节/内容页使用不同官方背景资产 |
| 识别特征 | 飞书官方花朵背景、顶部 wordmark、渐变 keyline、四级字号、透明卡片 |

## II. Color Scheme

| 角色 | 色值 | 用途 |
|---|---|---|
| Background Black | `#000000` | 页面底色、封底、深色框架 |
| Background Navy | `#04060F` | 内容页深色底 |
| Background Blue | `#0A1230` | 卡片层次与深蓝环境光 |
| Primary Blue | `#3C7FFF` | 主强调、关键数字、主卡片描边 |
| Cyan Highlight | `#24C3FF` | 关键词内联高亮 |
| Teal Accent | `#33D6C0` | 正向指标、渐变起点 |
| Purple Accent | `#5C3FFB` | 章节和重点卡片辅助强调 |
| Violet Accent | `#9F6FF1` | 光晕、结束页辅助色 |
| Orange Accent | `#FE7F00` | CTA、风险提示、少量暖色焦点 |
| Text Primary | `#FFFFFF` | 标题和正文主文字 |
| Text Secondary | `#B8C2D6` | 辅助说明 |
| Text Muted | `#7E89A8` | 来源、脚注、eyebrow |

## III. Typography

| 角色 | 字体栈 | 使用 |
|---|---|---|
| CJK | `"方正兰亭黑 Pro GB18030", "方正兰亭黑Pro_GB18030", "FZLanTingHeiPro_GB18030 Light", "PingFang SC", "Microsoft YaHei", sans-serif` | 标题、正文、卡片 |
| Latin | `"Inter", "Helvetica Neue", Arial, sans-serif` | 英文标签、数字、单位 |
| Mono | `"JetBrains Mono", "SF Mono", Menlo, Consolas, monospace` | 数据标签、技术角标 |

H5 原始画布为 1920×1080，迁移到 PPT Master `ppt169` 后按 2/3 缩放，并保留飞书四级字号秩序：标题约 32–48px，副标题约 22–28px，正文约 18–24px，脚注约 12–16px。

## IV. Signature Design Elements

| 元素 | 视觉表现 |
|---|---|
| 飞书官方背景 | `cover_bg.jpg`、`section_bg.jpg`、`content_bg.jpg` 分别用于封面/章节/内容页 |
| Wordmark | 飞书 logo 始终使用彩色版：内容/章节页右上角小号（约 `x=1090 y=41 w=107 h=33`），封面/结尾左上角大号；纯白版仅备用 |
| 渐变 keyline | `#33D6C0 → #3C7FFF → #5C3FFB`，用于顶部进度线、分割线、卡片焦点边 |
| 半透明卡片 | 深蓝卡片，白色 8–16% 描边，局部蓝色/紫色 8–16% 填充 |
| 产品式 mockup | 内容页右侧用窗口、面板、表格、消息气泡模拟产品截图，而不是普通图片框 |
| 严格网格 | 左右 96px H5 安全边距迁移为 64px，卡片采用 3 栏、4 栏、2 栏等稳定结构 |

## V. Page Roster

| 文件 | 类型 | 视觉与用途 |
|---|---|---|
| `01_cover.svg` | Cover | 官方花朵封面背景，左侧大标题，右侧保留品牌氛围图，适合客户提案封面 |
| `02_agenda.svg` | Agenda | 双列议程，蓝色编号 pill，适合 4–6 个章节目录 |
| `02_chapter.svg` | Chapter | 章节背景图、巨型章节号、产品能力 pill，适合章节分隔 |
| `03a_content_3up.svg` | Content 3up | 三张能力卡并列，蓝/紫/青三色轮换，适合三大能力/三支柱 |
| `03b_content_2col.svg` | Content 2col | 左文右产品面板 mockup，适合能力说明、流程叙事、产品演示 |
| `03c_content_quote.svg` | Quote | 居中大金句、渐变强调词、来源署名，适合客户原声或核心判断 |
| `03d_content_stats.svg` | Stats row | 四列 KPI 数字卡，适合量化结果和业务收益页 |
| `03e_content_big_stat.svg` | Big stat | 单个英雄数字 + 右侧解释，适合规模、效率、增长类高潮页 |
| `03f_content_table.svg` | Table | 深色对比表，蓝色主列高亮，内置样例对比维度，适合平台/方案/能力对比 |
| `03g_content_timeline.svg` | Timeline | 四阶段横向路径，内置周次与落地动作示例，适合 12 周落地、项目计划、实施路线 |
| `03h_content_logowall.svg` | Logo wall | 多行业客户 logo 墙区域，带行业标签与底部说明，适合客户实证、生态伙伴展示 |
| `04_ending.svg` | Ending | 官方封底背景、slogan、CTA 文案，适合正式收尾 |

## VI. Assets

| 文件 | 来源 | 用途 |
|---|---|---|
| `cover_bg.jpg` | `feishu-deck-h5/assets/lark-cover-bg.jpg` | 封面和封底背景 |
| `section_bg.jpg` | `feishu-deck-h5/assets/lark-section-bg.jpg` | 章节页背景 |
| `content_bg.jpg` | `feishu-deck-h5/assets/lark-content-bg.jpg` | 内容页背景 |
| `lark_logo.png` | `feishu-deck-h5/assets/lark-logo.png` | 彩色飞书 logo；封面、内容页、章节页和结尾页均使用彩色版 |
| `lark_logo_mono_white.png` | `feishu-deck-h5/assets/lark-logo-mono-white.png` | 保留备用；默认不用于本模板页面 |
| `lark_slogan.png` | `feishu-deck-h5/assets/lark-slogan.png` | 结尾页 slogan |

模板 SVG 为了保证任意工作目录下都能直接预览，已将这些背景和 logo 以内嵌 data URI 写入页面；保留同名源资产文件用于后续项目生成时复制到 `images/` 并按 `../images/<name>` 方式引用。

## VII. Placeholder Overrides

本模板沿用 PPT Master 常规占位符，但根据 `feishu-deck-h5` 的页面 recipe 增加 `KPI_*`、`FEATURE_*`、`STEP_*` 和 `VISUAL_TITLE` 等结构化 slot，方便后续 Strategist 根据内容选择对应页型。
