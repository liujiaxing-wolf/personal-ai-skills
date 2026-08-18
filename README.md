# Personal AI Skills

一组可以在 Codex、ChatGPT Skills 及其他兼容 Agent 中使用的个人技能包。

## 包含的技能

| Skill | 用途 | 来源 |
| --- | --- | --- |
| `agent-reach` | 互联网搜索与多平台内容读取路由 | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) |
| `humanizer-zh` | 中文去 AI 味、减少翻译腔与机械表达 | [ai-zixun/humanizer-zh](https://github.com/ai-zixun/humanizer-zh) |
| `human-writing` | 从想法扩散、研究和辩论到中文成稿、配图与复审 | 本仓库维护 |
| `reverse-user-journey` | 基于页面证据还原用户旅程、分支、情绪、痛点与机会点 | 本仓库维护 |
| `reverse-agent-contracts` | 识别可见 Agent 并拆解输入、判断、工具、输出和交接契约 | 本仓库维护 |
| `reconstruct-agent-prompt` | 为单个目标 Agent 编写可追溯的功能等价 System Prompt | 本仓库维护 |
| `reverse-product-architecture` | 综合 Agent、工具、上下文、资产、模型和治理形成产品架构 | 本仓库维护 |
| `reverse-ai-product-suite` | 编排上述四个逆向分析 Skill，并交付四份 HTML 报告 | 本仓库维护 |

## 安装到 Codex

```bash
git clone https://github.com/liujiaxing-wolf/personal-ai-skills.git
mkdir -p ~/.codex/skills
cp -R personal-ai-skills/skills/agent-reach ~/.codex/skills/
cp -R personal-ai-skills/skills/humanizer-zh ~/.codex/skills/
cp -R personal-ai-skills/skills/human-writing ~/.codex/skills/
cp -R personal-ai-skills/skills/reverse-user-journey ~/.codex/skills/
cp -R personal-ai-skills/skills/reverse-agent-contracts ~/.codex/skills/
cp -R personal-ai-skills/skills/reconstruct-agent-prompt ~/.codex/skills/
cp -R personal-ai-skills/skills/reverse-product-architecture ~/.codex/skills/
cp -R personal-ai-skills/skills/reverse-ai-product-suite ~/.codex/skills/
```

安装或更新后，请新建一个 Codex 任务，让技能清单重新加载。

`agent-reach` 目录提供 Agent 路由说明，完整的命令行能力仍需按照[上游安装文档](https://github.com/Panniantong/Agent-Reach#快速开始)配置相关工具。

## 安装到 ChatGPT Skills

将需要的 `skills/<skill-name>` 目录压缩为 ZIP，在 ChatGPT 的“插件 → 技能 → 创建/编辑 → 上传”中导入。不同运行环境提供的工具不同，因此本机命令、浏览器登录态和本地文件写入能力不会自动同步。

## 使用示例

```text
使用 $agent-reach 调研这个主题的公开资料和讨论。
使用 $humanizer-zh 把这篇中文稿改得更自然。
使用 $human-writing 从这个想法开始，陪我研究并完成一篇文章。
使用 $reverse-user-journey 基于截图还原这个产品的用户旅程。
使用 $reverse-agent-contracts 拆解页面中实际出现的所有 Agent 契约。
使用 $reconstruct-agent-prompt 为艺术总监编写功能等价 System Prompt。
使用 $reverse-product-architecture 输出完整的 AI 产品架构拆解。
使用 $reverse-ai-product-suite 一次完成四份 HTML 逆向分析报告。
```

## 许可与署名

本仓库的原创整理文件使用 MIT License。各技能目录内已有许可证的内容继续服从各自许可证。第三方来源、版权归属和修改说明见 [NOTICE.md](NOTICE.md)。

## 安全说明

仓库不包含 Cookie、API Key、账号令牌或浏览器数据。涉及登录态的平台，请只在自己的设备上完成授权，不要把凭据提交到仓库。
