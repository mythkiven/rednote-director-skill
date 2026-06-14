# 小红书高级图文视觉风格系统

## 默认审美基线

- 默认画幅：3:4 竖版，小红书手机端优先。
- 页面气质：高级、设计师审美、科技感、杂志感、极简但有冲击力。
- 信息结构：每页只承担一个主要任务，标题先抓住人，内页再给结构和证据。
- 字体：中文用思源黑体、阿里巴巴普惠体、HarmonyOS Sans、苹方风格；英文用 Inter、SF Pro、Helvetica Neue 风格。
- 色彩：黑、深灰、白、银灰为基础，可少量使用荧光绿、薄荷绿、电光蓝、亮橙、低饱和红。
- 禁止：廉价蓝紫渐变、随机霓虹线条、文字过小、PPT bullet 堆砌、塑料质感、儿童卡通感、巨大页码抢戏。

## 内容类型到风格映射表

| 内容类型 | 推荐风格 |
| --- | --- |
| AI / Vibe Coding / Agent 观点 | 深色科技杂志风；黑白灰 + 荧光绿冲击风；架构图 / 系统拆解风；赛博档案 / 黑客文件风 |
| 教程 / 方法论 / 知识拆解 | Notion 高级卡片风；课程讲义 / 高级黑板风；架构图 / 系统拆解风；高级白底杂志风 |
| 工具推荐 / 软件清单 | 高级工具清单风；Notion 高级卡片风；软件界面 UI 风；极简产品发布会风 |
| 商业 / 企业服务 / 产业方案 | 高级商业提案风；高级极简黑金风；全球贸易网络风；数据报告 / 趋势洞察风 |
| 个人品牌 / 账号定位 / 观点文章 | 个人品牌宣言风；高级白底杂志风；情绪共鸣 / 夜间独白风；黑白灰 + 荧光绿冲击风 |
| 产品图 / 商品图 / 电商详情 | 高级电商详情页风；极简产品发布会风；设计师灵感板风；高级商业提案风 |
| 设计改版 / 排版优化 | 设计师灵感板风；红绿对错对比风；高级白底杂志风；Notion 高级卡片风 |
| 数据 / 趋势 / 行业观察 | 数据报告 / 趋势洞察风；高级商业提案风；深色科技杂志风；高级白底杂志风 |
| 故事 / 漫画 / 隐喻表达 | 故事漫画分镜风；情绪共鸣 / 夜间独白风；反差冲击封面风 |

## 风格组合机制

- 封面可以更冲击，内页可以更理性：封面用反差冲击封面风，内页用架构图 / 系统拆解风，结尾用个人品牌宣言风。
- 教程类内容要增强收藏感：主风格 Notion 高级卡片风，辅助风格课程讲义 / 高级黑板风。
- AI 技术观点要避免太冷：主风格深色科技杂志风，辅助风格情绪共鸣 / 夜间独白风。
- 商业提案要避免太网感：主风格高级商业提案风，辅助风格全球贸易网络风。
- 产品展示要避免太 PPT：主风格高级电商详情页风，辅助风格极简产品发布会风。

## 按需读取规则

- 先用本文件完成内容类型到风格候选的匹配。
- 确定主风格和辅助风格后，只读取最终候选的 1-3 个 `references/style-XX-*.md` 文件。
- 不要一次性读取全部风格文件；需要生成图像提示词时，直接读取选定风格对应的小文件。
- 如果用户只问某个具体风格，只读取该风格文件和必要的审查规则。

## 24 种内置风格索引

| 编号 | 风格 | 适合内容速览 | 按需读取文件 |
| --- | --- | --- | --- |
| 1 | 深色科技杂志风 | AI、Vibe Coding、Agent、工具、认知升级、方法论、技术趋势。 | [style-01-dark-tech-magazine.md](./style-01-dark-tech-magazine.md) |
| 2 | 黑白灰 + 荧光绿冲击风 | 强观点、反常识、技术布道、个人观点、爆款封面。 | [style-02-mono-neon-green.md](./style-02-mono-neon-green.md) |
| 3 | Notion 高级卡片风 | 工具推荐、方法清单、工作流、资料整理、知识管理。 | [style-03-notion-cards.md](./style-03-notion-cards.md) |
| 4 | 液态玻璃 / 弥散极光风 | 产品发布、个人品牌、AI 应用、未来感选题、封面。 | [style-04-liquid-glass-aurora.md](./style-04-liquid-glass-aurora.md) |
| 5 | 极简产品发布会风 | 产品展示、工具介绍、个人项目发布、MVP 展示。 | [style-05-minimal-product-launch.md](./style-05-minimal-product-launch.md) |
| 6 | 反差冲击封面风 | 爆款封面、反常识观点、争议选题、强情绪开头。 | [style-06-contrast-cover.md](./style-06-contrast-cover.md) |
| 7 | 架构图 / 系统拆解风 | Agent 架构、产品系统、API Contract、工程化、复杂方法论。 | [style-07-system-architecture.md](./style-07-system-architecture.md) |
| 8 | 手机截图改造风 | App 工作流、桌面整理、工具教程、真实案例展示。 | [style-08-phone-screenshot-annotation.md](./style-08-phone-screenshot-annotation.md) |
| 9 | 高级商业提案风 | 企业服务、义乌商户、AI+产业、文旅方案、招商路演。 | [style-09-business-proposal.md](./style-09-business-proposal.md) |
| 10 | 全球贸易网络风 | 义乌、外贸、跨境电商、全球化、供应链、物流。 | [style-10-global-trade-network.md](./style-10-global-trade-network.md) |
| 11 | 高级白底杂志风 | 认知文章、审美分享、个人观点、理性内容。 | [style-11-white-magazine.md](./style-11-white-magazine.md) |
| 12 | 红绿对错对比风 | 错误示范 vs 正确示范、Prompt 优化、设计改版。 | [style-12-red-green-comparison.md](./style-12-red-green-comparison.md) |
| 13 | 赛博档案 / 黑客文件风 | Agent、自动化、代码工具、实验复盘、技术探索。 | [style-13-cyber-dossier.md](./style-13-cyber-dossier.md) |
| 14 | 未来实验室风 | AI 实验、产品原型、未来工具、概念验证。 | [style-14-future-lab.md](./style-14-future-lab.md) |
| 15 | 设计师灵感板风 | 审美教程、页面改版、封面风格选择、设计技巧。 | [style-15-designer-moodboard.md](./style-15-designer-moodboard.md) |
| 16 | 高级极简黑金风 | 商业、品牌、成交、课程、咨询、企业方案。 | [style-16-minimal-black-gold.md](./style-16-minimal-black-gold.md) |
| 17 | 软件界面 UI 风 | AI 产品、SaaS、工具、工作台、自动化流程。 | [style-17-software-ui.md](./style-17-software-ui.md) |
| 18 | 课程讲义 / 高级黑板风 | 教程、知识科普、课程系列、Day 系列。 | [style-18-premium-blackboard.md](./style-18-premium-blackboard.md) |
| 19 | 个人品牌宣言风 | 自我介绍、账号定位、观点输出、个人 IP。 | [style-19-personal-brand-manifesto.md](./style-19-personal-brand-manifesto.md) |
| 20 | 情绪共鸣 / 夜间独白风 | 个人思考、创业感悟、AI 时代焦虑、成长内容。 | [style-20-night-monologue.md](./style-20-night-monologue.md) |
| 21 | 数据报告 / 趋势洞察风 | 行业趋势、研究结论、市场洞察、案例分析。 | [style-21-data-report.md](./style-21-data-report.md) |
| 22 | 故事漫画分镜风 | 用故事讲复杂概念、AI 与人类关系、讽刺漫画、轻量表达。 | [style-22-story-comic-panels.md](./style-22-story-comic-panels.md) |
| 23 | 高级电商详情页风 | 产品图改造、义乌商品、AI 商品图、包装设计、详情页头图。 | [style-23-premium-ecommerce-detail.md](./style-23-premium-ecommerce-detail.md) |
| 24 | 高级工具清单风 | 软件推荐、AI 工具合集、效率工具、工作流。 | [style-24-premium-tool-list.md](./style-24-premium-tool-list.md) |
