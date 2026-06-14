# 图像提示词模板索引

使用方式：先读取 `references/style_system.md` 判断候选风格，再只读取选定风格对应的 `references/style-XX-*.md`。每个风格文件已经包含该风格的适用范围、版式结构、图像提示词模板和负面提示词。

不要为了生成单个提示词而加载全部 24 种风格。除非用户明确要求横向比较全部风格，否则最多读取 1-3 个候选风格文件。

## 通用负面提示词

```text
不要廉价蓝紫渐变，不要随机霓虹线条，不要文字变形，不要小字堆积，不要 PPT bullet 列表，不要塑料质感，不要儿童卡通，不要低清晰度，不要过度装饰，不要元素遮挡标题，不要页码喧宾夺主。
```

## 按需模板索引

| 编号 | 风格 | 图像提示词模板位置 |
| --- | --- | --- |
| 1 | 深色科技杂志风 | [references/style-01-dark-tech-magazine.md](../references/style-01-dark-tech-magazine.md) |
| 2 | 黑白灰 + 荧光绿冲击风 | [references/style-02-mono-neon-green.md](../references/style-02-mono-neon-green.md) |
| 3 | Notion 高级卡片风 | [references/style-03-notion-cards.md](../references/style-03-notion-cards.md) |
| 4 | 液态玻璃 / 弥散极光风 | [references/style-04-liquid-glass-aurora.md](../references/style-04-liquid-glass-aurora.md) |
| 5 | 极简产品发布会风 | [references/style-05-minimal-product-launch.md](../references/style-05-minimal-product-launch.md) |
| 6 | 反差冲击封面风 | [references/style-06-contrast-cover.md](../references/style-06-contrast-cover.md) |
| 7 | 架构图 / 系统拆解风 | [references/style-07-system-architecture.md](../references/style-07-system-architecture.md) |
| 8 | 手机截图改造风 | [references/style-08-phone-screenshot-annotation.md](../references/style-08-phone-screenshot-annotation.md) |
| 9 | 高级商业提案风 | [references/style-09-business-proposal.md](../references/style-09-business-proposal.md) |
| 10 | 全球贸易网络风 | [references/style-10-global-trade-network.md](../references/style-10-global-trade-network.md) |
| 11 | 高级白底杂志风 | [references/style-11-white-magazine.md](../references/style-11-white-magazine.md) |
| 12 | 红绿对错对比风 | [references/style-12-red-green-comparison.md](../references/style-12-red-green-comparison.md) |
| 13 | 赛博档案 / 黑客文件风 | [references/style-13-cyber-dossier.md](../references/style-13-cyber-dossier.md) |
| 14 | 未来实验室风 | [references/style-14-future-lab.md](../references/style-14-future-lab.md) |
| 15 | 设计师灵感板风 | [references/style-15-designer-moodboard.md](../references/style-15-designer-moodboard.md) |
| 16 | 高级极简黑金风 | [references/style-16-minimal-black-gold.md](../references/style-16-minimal-black-gold.md) |
| 17 | 软件界面 UI 风 | [references/style-17-software-ui.md](../references/style-17-software-ui.md) |
| 18 | 课程讲义 / 高级黑板风 | [references/style-18-premium-blackboard.md](../references/style-18-premium-blackboard.md) |
| 19 | 个人品牌宣言风 | [references/style-19-personal-brand-manifesto.md](../references/style-19-personal-brand-manifesto.md) |
| 20 | 情绪共鸣 / 夜间独白风 | [references/style-20-night-monologue.md](../references/style-20-night-monologue.md) |
| 21 | 数据报告 / 趋势洞察风 | [references/style-21-data-report.md](../references/style-21-data-report.md) |
| 22 | 故事漫画分镜风 | [references/style-22-story-comic-panels.md](../references/style-22-story-comic-panels.md) |
| 23 | 高级电商详情页风 | [references/style-23-premium-ecommerce-detail.md](../references/style-23-premium-ecommerce-detail.md) |
| 24 | 高级工具清单风 | [references/style-24-premium-tool-list.md](../references/style-24-premium-tool-list.md) |
