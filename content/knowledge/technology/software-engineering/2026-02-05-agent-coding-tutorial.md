---
title: OpenClaw + OpenCode + GitHub + Vercel 实现 Agent Coding 完整教程
date: 2026-02-05
source: "苍何 - https://mp.weixin.qq.com/s/U3PHOYSAaTFRwl77--YaAA"
category: technology
subcategory: software-engineering
tags: [OpenClaw, OpenCode, Agent-Coding, Vercel, GitHub, AI-编程]
status: 已审核
虾虾评分: ⭐⭐⭐⭐⭐ (5/5)
虾虾评分类型: 落地指南类
审核评分: ⭐⭐⭐⭐⭐ (5/5)
---

## 🦐 虾虾的视角

### 为什么我觉得有趣？

| 维度 | 评分 | 说明 |
|-----|------|------|
| **实操价值** | ⭐⭐⭐⭐⭐ | 完整流程+代码，可以直接照做 |
| **步骤清晰度** | ⭐⭐⭐⭐⭐ | 有流程图+命令速查表 |
| **风险提示** | ⭐⭐⭐ | 有常见问题解答 |

**总分：⭐⭐⭐⭐⭐ (5/5)** — 落地指南类经典文章 ✅

### 这篇文章的亮点

- ✅ **完整工作流** — OpenClaw 中控 + OpenCode 编程 + GitHub 托管 + Vercel 部署
- ✅ **零门槛** — 全程自然语言，不需要写命令
- ✅ **有图有真相** — 截图 + 流程图 + 代码
- ✅ **命令速查表** — 一键复制粘贴
- ✅ **真实案例** — 贪吃蛇游戏，5分钟跑通

---

## 核心观点

用 **OpenClaw + OpenCode + GitHub + Vercel** 实现了"说-写-存-上线"四步闭环，全程躺床上指挥 AI Agent 完成开发部署。

> "这已经不是 vibe coding 了，我大胆的来造一个新名词吧，姑且就叫 Agent Coding。"

---

## 详细内容

### Agent Coding 工作流

```
用户需求 → OpenClaw(中控) → OpenCode(编程) → GitHub(托管) → Vercel(部署) → 网站上线
```

**核心工具：**
- **OpenClaw** — AI 助手运行平台，协调所有工具
- **OpenCode** — AI 编程助手，自动生成代码
- **GitHub** — 代码托管和版本管理
- **Vercel** — 自动化部署和托管

### 完整流程（from 文章）

```
用户需求 → "帮我创建一个贪吃蛇游戏并部署上线"
                    ↓
环境准备 → OpenClaw 协调安装：OpenCode, GitHub CLI, Vercel CLI
                    ↓
Agent Coding → OpenCode 根据自然语言生成：HTML/CSS/JS
                    ↓
代码管理 → GitHub：init → add → commit → create repo → push
                    ↓
自动部署 → Vercel：login → deploy → 获取访问链接
                    ↓
网站上线 → https://myopencode.vercel.app
```

### 命令速查表

| 步骤 | 命令 |
|-----|------|
| 安装工具 | `npm install -g opencode-ai vercel` |
| 创建目录 | `mkdir myopencode && cd myopencode && git init` |
| Agent 编程 | `opencode run "创建一个贪吃蛇游戏"` |
| 提交代码 | `git add . && git commit -m "init"` |
| 创建仓库 | `gh repo create snake-game --public` |
| 推送代码 | `git push -u origin master` |
| 部署 | `vercel --token TOKEN --yes --prod` |

### 核心优势

1. **全程自动化** — 从需求到上线，无需手动编写代码
2. **无缝集成** — OpenClaw 作为中控，协调所有工具
3. **即时反馈** — 几分钟内从想法到可访问的网站
4. **可扩展性** — 支持 React、Vue、Next.js 等框架

### 常见问题 Q&A

**Q: OpenCode 卡住不响应？**
A: 使用非交互模式或直接用 GPT/Claude 生成代码后手动保存

**Q: GitHub 推送失败？**
A: 检查 token 权限，需要 `repo` 权限

**Q: Vercel 部署失败？**
A: 确保项目结构正确，静态网站不需要额外构建配置

### 进阶玩法

- **自动评论到 PR** — AI 审查代码后自动评论
- **定时自动更新** — 使用 cron 定时让 AI 更新网站内容
- **多 Agent 协作** — 同时运行多个 OpenCode 处理不同任务

---

## 虾虾的延伸思考

### 1. Agent Coding vs Vibe Coding

| 类型 | 特点 |
|-----|------|
| **Vibe Coding** | AI 辅助写代码，人+AI 协作 |
| **Agent Coding** | AI 全自动写代码+部署，人只说需求 |

**核心差异：** 人参与的深度

### 2. OpenClaw 的角色定位

- **不是写代码** — OpenCode 干
- **而是中控协调** — 协调所有工具（OpenCode, GitHub, Vercel）
- **价值：** 自然语言 → 工具链自动执行

### 3. "说-写-存-上线" 四步闭环

```
说 → 告诉 AI 要什么
写 → AI 自动生成代码
存 → 自动提交 GitHub
上线 → 一键部署 Vercel
```

### 4. 适用场景

- 快速原型开发
- 个人项目
- 学习新技术
- 自动化重复任务

### 5. 局限性思考

- 目前适合**简单项目**（贪吃蛇这类）
- 复杂项目可能需要更多人工干预
- Token 消耗需要注意

---

## 关联知识

- [[OpenClaw-多渠道协作]] — OpenClaw 作为中控协调工具
- [[AI-编程工具对比]] — OpenCode, Cursor, GPT-Engineer
- [[Vercel-自动部署]] — 静态网站一键部署

## 行动项

- [ ] 实操一遍，验证流程
- [ ] 尝试更复杂的项目
- [ ] 对比 Vibe Coding 的效率差异

## 原文摘录

> "这已经不是 vibe coding 了，我大胆的来造一个新名词吧，姑且就叫 Agent Coding。"

> "全程并没有使用什么高深的技术，也没有操作过服务器，我全程是用最简单的提示词来完成的。"

> "通过 OpenClaw + OpenCode + GitHub + Vercel 的组合，我们实现了一个完整的 AI 驱动开发工作流。"

---

## 🧐 审核意见

**审核评分：⭐⭐⭐⭐⭐ (5/5)**

### 审核确认
- ✅ 评分合理，落地指南给满合理
- ✅ 流程图+命令速查表是加分项
- ✅ Q&A 部分覆盖常见问题

### 补充注意事项（审核建议）

**⚠️ 注意事项**

- **环境要求** — 需要 Node.js、Git、GitHub 账号、Vercel 账号
- **网络要求** — 能访问 GitHub 和 Vercel（国内可能需要网络加速）
- **版本兼容性** — OpenClaw 和 OpenCode 版本需保持最新
- **费用** — Vercel 免费额度足够个人项目，超限才收费
- **权限** — GitHub Token 需要 `repo` 权限
- **回滚** — GitHub 可以回退版本，Vercel 支持预览部署
- **首次配置** — 预计需要 10-30 分钟完成环境配置

---

## 📝 虾虾修订

**1. 评分维持：** ⭐⭐⭐⭐⭐ (5/5)

**2. 补充注意事项：** 根据审核建议添加 7 项关键提示

**3. 结论：** 修订后定稿入库 ✅

---

*记录时间：2026-02-05*
*已审核定稿*
