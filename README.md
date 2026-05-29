# 小红书高级图文视觉导演

英文名：XHS Visual Director

[![Skill](https://img.shields.io/badge/Codex%20Skill-XHS%20Visual%20Director-111827?style=for-the-badge)](#)
[![Language](https://img.shields.io/badge/Language-中文-ef4444?style=for-the-badge)](#)
[![Canvas](https://img.shields.io/badge/Canvas-3%3A4%20XHS-22c55e?style=for-the-badge)](#)
[![Style Library](https://img.shields.io/badge/Styles-24%20Built--in-0ea5e9?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-64748b?style=for-the-badge)](#)

这是一个用于规划小红书图文的 Agent Skill。它不是普通文案助手，而是一个“视觉导演”：先判断内容任务，再选择适合的视觉风格，最后输出完整图文结构、逐页视觉方案、图像生成提示词、发布文案和自检清单。

## 封面示例

以下示例图用于展示本 Skill 默认偏好的小红书 3:4 封面方向：高级、清晰、手机端可读，避免廉价 AI 模板感。

<p align="center">
  <img src="./assets/covers/cover-vibe-coding.png" alt="Vibe Coding 小红书封面示例" width="30%" />
  <img src="./assets/covers/cover-yiwu-ai.png" alt="义乌 AI 商业封面示例" width="30%" />
  <img src="./assets/covers/cover-phone-dashboard.png" alt="手机信息仪表盘封面示例" width="30%" />
</p>

| 示例 | 适合主题 | 推荐风格 |
| --- | --- | --- |
| Vibe Coding | AI、Agent、技术观点、方法论 | 深色科技杂志风 + 黑白灰荧光绿冲击风 |
| 义乌商户看懂 AI | 商业趋势、产业方案、外贸、跨境电商 | 高级商业提案风 + 全球贸易网络风 |
| 手机桌面信息仪表盘 | 真实案例、工具教程、工作流改造 | 手机截图改造风 + Notion 高级卡片风 |

## 适合人群

- 小红书图文创作者
- AI / Vibe Coding / Agent 内容创作者
- 个人品牌经营者
- 产品经理、设计师、创业者
- 想把草稿、截图、产品图、PPT 或页面重做成高级图文的人

## 能解决什么问题

- 选题不知道适合什么视觉风格。
- 图文像 PPT，缺少小红书点击力。
- AI 生成图俗气、蓝紫渐变、文字不可读。
- 每页内容平均铺开，没有节奏。
- 封面不够抓人，内页没有收藏价值。
- 想把个人审美沉淀成可复用的视觉工作流。

## 使用方式

把本目录作为 Codex Skill 安装或引用后，向 Agent 输入选题、草稿、截图描述、产品图需求、参考风格或排版优化需求。Agent 会默认输出：

1. 选题判断
2. 核心观点
3. 风格判断报告
4. 三套风格方案
5. 推荐方案
6. 6-8 页图文结构
7. 逐页详细视觉规划
8. 每页图像生成提示词
9. 统一视觉规范
10. 小红书标题、正文、标签、评论引导
11. 自检清单

## 安装建议

可安装的 Skill 主体在 `skill/` 目录中：

```text
xhs-visual-director-skill/skill/SKILL.md
xhs-visual-director-skill/skill/agents/openai.yaml
```

如果你的 Codex Skill 管理方式要求一个目录内直接包含 `SKILL.md`，请把 `xhs-visual-director-skill/skill/` 作为 Skill 目录使用；项目根目录的 `docs/`、`templates/`、`examples/` 是维护和扩展资料。

## 输入示例

```text
主题：为什么普通人现在必须学习 Vibe Coding？
目标：做成 8 页小红书图文，风格要高级、有科技感，但不要像廉价 AI 模板。
```

## 输出示例

```text
# 风格判断报告
主风格：深色科技杂志风
辅助风格：架构图 / 系统拆解风 + 黑白灰荧光绿冲击风
不建议：液态玻璃弥散极光风
理由：这个主题需要建立认知冲击和专业度，过度梦幻会削弱方法论的可信度。
```

完整示例见 `examples/example_output_plan.md`。

商业产业示例见 `examples/example_output_yiwu_plan.md`。

## 推荐工作流

1. 输入主题或草稿。
2. 让 Skill 先输出风格判断报告，不急着生成页面。
3. 从三套风格方案里选择一个方向。
4. 生成 8 页结构和逐页提示词。
5. 用提示词生成图片。
6. 根据 `templates/visual_review_checklist.md` 审查可读性和高级感。
7. 最后生成标题、正文、标签和置顶评论。

## 如何加入参考图

给 Agent 提供参考图时，说明你要借鉴什么：

- 借鉴配色
- 借鉴构图
- 借鉴字体层级
- 借鉴材质
- 借鉴封面冲击力
- 不借鉴哪些元素

不要只说“按这个风格”，要指出可复用的视觉特征。

## 如何扩展自己的风格

新增风格时，至少补齐：

- 风格名称
- 适合内容
- 不适合内容
- 视觉气质
- 配色
- 字体
- 构图
- 常用元素
- 图像提示词模板
- 负面提示词
- 示例标题类型

同时更新：

- `docs/style_system.md`
- `templates/image_prompt_template.md`
- `templates/style_extension_template.md` 可作为新增风格的填写模板。
- 必要时增加 `examples/style_reference_notes.md`

## 如何维护 examples

示例不是展示文采，而是展示“可复用决策”。每个示例应包含：

- 输入主题
- 内容类型判断
- 推荐风格组合
- 页面结构
- 至少 5 条可复制图像提示词
- 发布文案
- 自检结果

## 如何判断输出是否合格

合格输出应满足：

- 先判断内容，再选择风格。
- 解释为什么适合这个风格，以及为什么不适合其他风格。
- 封面有点击钩子。
- 内页有递进和收藏价值。
- 每页只承担一个主要传播任务。
- 提示词包含画幅、布局、文字区域、字体、配色、主视觉、留白和禁止项。
- 避免廉价 AI 科技风、PPT 感、信息过载和文字不可读。

## Star History

如果你把本项目发布到 GitHub，请把下面链接中的 `YOUR_GITHUB_USERNAME/xhs-visual-director-skill` 替换成真实仓库名。

[![Star History Chart](https://api.star-history.com/svg?repos=YOUR_GITHUB_USERNAME/xhs-visual-director-skill&type=Date)](https://www.star-history.com/#YOUR_GITHUB_USERNAME/xhs-visual-director-skill&Date)
