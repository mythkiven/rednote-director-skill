# AGENTS.md

本项目不是“小红书文案模板库”，而是一个“小红书高级图文视觉导演 Agent Skill”。

## 维护原则

- 修改这个 Skill 时，优先维护 `skill/SKILL.md`。
- 所有规则必须服务于“小红书高级图文视觉导演”这个定位。
- 不要把 Skill 写成泛泛的写作助手。
- 不要输出空泛审美词，例如只写“高级、科技、极简、好看”。
- 所有示例都要具体到页面任务、信息层级、构图、配色、字体和图像提示词。
- 所有模板都要可直接复制使用。
- 中文是默认语言。
- 文件结构必须清晰，新增内容要放到对应目录。
- `README.md` 要告诉用户如何使用这个 Skill，而不是只介绍概念。
- 风格库必须可扩展。
- 新增风格时必须同时更新 `docs/style_system.md` 和 `templates/image_prompt_template.md`。
- 任何输出都必须先判断内容，再选择风格。
- 不要默认套黑色科技风。
- 不要把可读的风格判断报告写成隐藏思考链。

## 文件职责

- `skill/SKILL.md`：Agent 的触发场景、工作流、默认输出格式、审查规则。
- `skill/agents/openai.yaml`：Codex UI 元数据；当 Skill 名称、定位或默认使用方式变化时同步更新。
- `docs/style_system.md`：风格库、风格组合规则、内容类型到风格的映射表。
- `docs/page_structure_rules.md`：封面、内页、结尾页的页面结构规则。
- `docs/prompt_rules.md`：图像生成提示词写法、负面提示词规则、文字区域规划。
- `docs/anti_patterns.md`：用户不喜欢的风格和避免方法。
- `templates/`：可复用输出模板。
- `examples/`：可复用案例，新增案例必须具体、完整、可模仿。

## 输出底线

一个合格输出必须同时回答：

1. 这篇内容是什么类型。
2. 传播目标是什么。
3. 读者应该产生什么情绪。
4. 为什么选这个风格。
5. 为什么不选某些风格。
6. 封面如何抓点击。
7. 内页如何递进并产生收藏价值。
8. 每页的视觉方案如何落地。
9. 图像生成提示词如何直接复制使用。
10. 发布文案如何引导收藏、评论和关注。

## 新增风格要求

新增风格时，先使用 `templates/style_extension_template.md` 填完整，再同步更新：

- `docs/style_system.md`
- `templates/image_prompt_template.md`
- `examples/style_reference_notes.md`

如果新增风格面向一个明确行业，例如外贸、电商、教育、咨询、文旅，至少补一个行业主题案例到 `examples/`。
