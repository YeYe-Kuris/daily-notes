---
title: 任务追踪
date: 2026-02-04
updated: 2026-03-02
tags: [todo, tracking]
---

# 📋 任务追踪板

## 🟡 进行中 (In Progress)
| 任务 | 状态 | 备注 | 截止日期 |
|------|------|------|----------|
| ADB 手机方案开发 | 进行中 | core.py 防风控层已完成，等新号认证 | - |
| Kuris persona 系统 Phase 1 | 进行中 | core.json + quirks.json + prompt_builder 已完成，通知监听已跑通 | - |
| xhs2 小德日常运营（浏览器） | 运行中 | 巡逻 + 回评论 cron 持续运行；已加 tab 清理/focus/超时恢复，10:03 轮次巡逻已恢复（browsed=3, favorited=1） | 持续 |
| 小红书运营 skill 产品化 | 进行中 | 已输出产品化方案 v0：reports/xhs-skill-productization-v0-2026-03-02.md，进入 M1 实装拆分 | - |
| Agent 替人筛选设计（idea） | 进行中 | 已输出方案 v0：reports/agent-screening-design-v0-2026-03-01.md | - |
| 模型分层效果监控 | 进行中 | 已追加 07:00 检查点：reports/model-tier-monitoring-2026-03-01.md，memory_search 401 作为当前风险项跟踪 | 持续 |
| 自动化运营 toB 方向验证 | 进行中 | 已补齐首批访谈包：reports/tob-validation-interview-pack-v0-2026-03-02.md，待执行访谈预约 | - |
| Kuris 视频 Pipeline（15s） | 进行中 | 已新增 Seedance 输入模板：projects/kuris-video-pipeline/storyboard-v2-seedance-template.md，待单条实测 | - |
| 粉丝关系系统 | 进行中 | 已补 v0.2 接入映射草案（字段映射+闸门插入位）：reports/fan-relationship-system-v0-2026-03-01.md，下一步接入 xhs2 流水 | - |
| 多平台 Agent 架构 | 进行中 | 已输出架构草案：reports/multi-platform-agent-architecture-v0-2026-03-01.md，待拆分平台 PoC | - |
| Agent-Reach 夜间基线对照（7天） | 进行中 | 已接入 nightly probe（23:20），首轮 6/12，目标验证是否能互补 Kuris brain | 2026-03-09 |
| TODO 记忆维护（日更） | 进行中 | 已恢复 memory_search 驱动维护机制（07:40 cron），用于回填和纠偏 tasks.md | 持续 |

## ❌ 待办 (Todo)

### 🔴 高优先级
| 任务 | 阻塞原因 | 下一步动作 |
|------|----------|------------|
| ADB：新号认证通过后首测 | 等认证 | 纯 adb 方案跑巡逻，验证防风控效果 |
| ADB：patrol.py 适配纯 adb | 待开发 | 去掉 uiautomator2 依赖，用 core.py |
| xhs2 Web 对外产品化（30账号并发） | 待方案评审 | 先用 2 账号试点调试，完善稳定性与风控后再扩到 30 账号 |
| xhs2 回评论重复回复回归观察（DeepRead Planet） | 需连续观测 | 观察 3-5 轮 run，确认无 self_echo 与同用户连回 |
| ADB 方案产品化（MCP/SaaS） | 先验证封号风险 | persona 模板化 + 多账号支持 + Web Dashboard，给 MCN 用 |

### 🟡 中优先级
| 任务 | 阻塞原因 | 下一步动作 |
|------|----------|------------|
| ADB：私信功能开发 | ✅ 基本完成 | settext.dex 中文输入 + processor.py 自动回复 |
| ADB：通知驱动自动回复 | 进行中 | watcher.py 已跑通，processor.py 已接入 LLM |
| ADB：publish.py 适配纯 adb | 待开发 | 发笔记流程用 core.py 重写 |

### 🟢 低优先级 / 后续
| 任务 | 说明 |
|------|------|
| sendevent 触摸方案 | 需要 root，暂不做。root 后可启用内核级零痕迹触摸 |

### 🎮 独立游戏（长线项目）
| 任务 | 说明 |
|------|------|
| 游戏概念文档 | "天上的鸟都是无人机" — 表面星露谷式田园种田，暗线楚门世界监控社会。玩家逐渐发现鸟飞行路线太规律、村民对话有重复、信号干扰等线索，真相浮出水面 |
| 技术选型调研 | 引擎选择（Godot/Unity）、AI 辅助美术/音乐方案 |
| 原型 Demo | 先做一个最小可玩版本验证核心玩法 |
| 开发过程做内容 | "一个人用 AI 做独立游戏"系列，发小红书/B站，游戏和自媒体互相喂养 |

## ✅ 已完成 (Done)
| 任务 | 完成时间 | 备注 |
|------|----------|------|
| A2A 抗碰撞策略 v3.2 更新 | 2026-03-02 | 已补 A2H Bridge Mode + 短板清单并推送：projects/agent2agent/A2A_AntiCollision_Strategy.md |
| codex-bridge 沙盒（Obsidian结构归集）实操 | 2026-03-02 | 链路跑通并落盘评估：reports/codex-20260302-093531/bridge_sandbox_evaluation.md |
| Agent-Reach 方案A二次评测 | 2026-03-02 | Python 3.11+ 官方安装路径验证通过，doctor 当前 6/12 |
| Kuris character-profile.json | 2026-03-01 | 已完成并落盘：projects/kuris-video-pipeline/character-profile.json |
| Kuris 角色定义图锁定（v1） | 2026-03-01 | 已锁定主参考图：projects/kuris-video-pipeline/reference-image-lock.md |
| ADB：actions.py 操作顺序随机化 | 2026-03-01 | 已在 projects/adb-xhs/actions.py 落地 random.shuffle，互动顺序不再固定 |
| 即时热点快评执行手册 v0 | 2026-03-01 | 已输出：reports/hot-topic-fast-comment-playbook-v0-2026-03-01.md |
| 运营策略文档 | 2026-03-01 | 已输出初版：reports/xhs-ops-strategy-v0-2026-03-01.md |
| 抖音 ADB 脚本化与文档 | 2026-03-01 | 已输出合规稳定版脚本，含轨迹扰动与包名校验，存放在 projects/douyin-adb-safe |
| xhs2 回评论防重升级 | 2026-02-26 | 已加通知结构防误判 + self_echo 过滤 + 同用户单轮1条 + 去重路径锁定 |
| xhs2 回评论 Kuris brain 挂载 | 2026-02-26 | 启用任务前置读取 PERSONA/MEMORY/STRATEGY/VOICE + VOICE.runtime.json |
| settext.dex 零 APK 中文输入 | 2026-02-22 | UiAutomation ACTION_SET_TEXT，替代 clip.dex |
| Kuris persona 文件系统 | 2026-02-22 | core.json + quirks.json + world-info + prompt_builder.py |
| 通知监听 watcher.py | 2026-02-22 | dumpsys + 截图红点双模式，SQLite 队列 |
| ADB core.py 防风控层 | 2026-02-20 | 贝塞尔滑动、疲劳模型、误操作、safety_check |
| clip.dex 中文输入方案 | 2026-02-20 | app_process + 剪贴板粘贴，零 APK |
| sendevent 可行性验证 | 2026-02-20 | SELinux 阻止，需 root，暂不用 |
| Codex 审查 core.py | 2026-02-20 | P0/P1/P2 改进建议，已落地 P0+P1 |
| 多平台筛选与评估 | 2026-02-17 | 小红书 > B站 > 即刻 > 抖音 > X |
| xhs2 小德账号搭建 | 2026-02-15 | 浏览器方案运行中 |
| 模型分层成本优化 | 2026-02-16 | 日成本从 $100+ 降到 $15-35 |
| 蹭流策略上线 | 2026-02-10 | 甜区 30-500 赞 |
| 知识库重构 | 2026-02-04 | 完成分类结构调整 |

---

## 🎬 Kuris 抖音视频 Pipeline — 任务拆解

**方案：Kuris 参考图 + 文字分镜 → Seedance 2.0 生成视频**
**第一条视频：Kuris 的第一条 vlog（15s，7 镜头）**

### Phase 1：素材准备
| # | 任务 | 优先级 | 状态 | 说明 |
|---|------|--------|------|------|
| 1.1 | 确定 Kuris 角色定义图 | 🔴 高 | ✅ 已完成 | 已锁定主参考图：media/kuris-newyear.png（见 reference-image-lock.md） |
| 1.2 | 编写 character-profile.json | 🔴 高 | ✅ 已完成 | 角色描述卡已落盘：projects/kuris-video-pipeline/character-profile.json |
| 1.3 | 完善分镜脚本 | 🔴 高 | ✅ v2 已补齐 | 新增 Seedance 输入模板：projects/kuris-video-pipeline/storyboard-v2-seedance-template.md，待实测 |

### Phase 2：视频生成
| # | 任务 | 优先级 | 状态 | 说明 |
|---|------|--------|------|------|
| 2.1 | 注册/登录即梦 AI | 🔴 高 | 待做 | 确认 Seedance 2.0 可用 |
| 2.2 | 测试单镜头生成 | 🔴 高 | 待做 | 先测镜头 2 |
| 2.3 | 逐镜头生成 | 🔴 高 | 待做 | 按分镜逐个生成 |

### Phase 3：后期合成
| # | 任务 | 优先级 | 状态 | 说明 |
|---|------|--------|------|------|
| 3.1 | 视频拼接 + 转场 | 🔴 高 | 待做 | FFmpeg |
| 3.2 | 配音生成 | 🔴 高 | 待做 | TTS 女声旁白 |
| 3.3 | 配乐 + 字幕 | 🟡 中 | 待做 | BGM + 环境音 + 字幕 |

### Phase 4：发布
| # | 任务 | 优先级 | 状态 | 说明 |
|---|------|--------|------|------|
| 4.1 | 抖音账号准备 | 🔴 高 | 待做 | Kuris 抖音账号 |
| 4.2 | 发布 + 互动 | 🔴 高 | 待做 | 标题、标签、封面 |
