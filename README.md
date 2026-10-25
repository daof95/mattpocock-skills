# mattpocock/skills（收藏）

> 本仓库是个人收藏的软件工具介绍页。工具本体由原作者维护：**https://github.com/mattpocock/skills**

## 是什么

TypeScript 圈知名开发者 Matt Pocock（《Total TypeScript》作者）开源的 AI 编码 Agent 技能集「Skills For Real Engineers」，把他日常使用的工程实践压缩成一个个可独立调用的小技能，解决 AI 编程四大痛点：

| 痛点 | 对应技能 |
|---|---|
| 需求没说清 AI 就开写 | `/grill-with-docs`、`/grill-me`（AI 反过来追问你） |
| AI 表达啰嗦、不懂项目术语 | CONTEXT.md 领域术语词典 + ADR 架构决策记录 |
| 代码跑不通、没测试 | `/tdd`（强制红-绿-重构）、`/diagnose`（先复现再假设） |
| 代码越写越腐化 | `/improve-codebase-architecture`（扫描+改进建议） |

## 特色

- **小而可组合**：不是大而全流程框架，每个技能粒度小，可单独选用、改造
- **模型无关**：适配 Claude Code、Codex、Cursor 等支持 Agent Skills 规范的工具
- **完整链路**：`/to-spec` → `/to-tickets` → `/implement` → `/code-review` 串成端到端工作流
- **安全护栏**：`/git-guardrails-claude-code` 拦截 force push 等危险 git 命令

## 安装

```bash
# 方式一：插件市场（自动更新）
claude plugins install mattpocock-skills

# 方式二：技能文件落盘（可本地修改）
npx skills@latest add mattpocock/skills
```

安装后每个仓库跑一次 `/setup-matt-pocock-skills` 做初始配置。

## 评价与注意

- MIT 协议；约 23 万 star、1800 万+ 累计安装量，是安装量最高的技能集，口碑极佳
- 适合所有重度使用 AI 编程工具、想给工作流加"工程护栏"的开发者
- 注意：插件版和落盘版二选一，都装会技能重复

## 相关链接

- 工具本体：https://github.com/mattpocock/skills
- 技能市场：https://skills.sh
