# bamboo-ceiling-career

**沟通**（会议发言 / 表达异议 / 向上沟通）、**晋升**（成果归档 / 绩效讨论 / 导师与成长机会）、
**求职**（岗位定位 / 面试表达 / 人脉交流）。

18 张能力卡 + 1 个入口 + 3 个参考件，**完全自包含、离线可用**：每张卡自带规则要点、案例、
应用与执行清单、边界与失效条件，不需要任何外部资料、量表或链接即可执行。

## 安装

把 `bamboo-ceiling-career/` 整个目录放进宿主的 skills 目录即可（不要只放 `SKILL.md`，能力卡在 `references/` 下）：

```text
~/.codex/skills/bamboo-ceiling-career/
~/.claude/skills/bamboo-ceiling-career/
<project>/.claude/skills/bamboo-ceiling-career/
```

```text
bamboo-ceiling-career/
├── SKILL.md                      # 入口：触发条件、核心原则、能力路由表、判停条件
├── BUILD_MANIFEST.json
└── references/
    ├── capabilities/*.md         # 18 张能力卡（R / I / A1 / A2 / E / B 六段）
    ├── capability-index.md       # 完整意图与关键词索引
    ├── cheatsheet.md             # 决策规则速查（一句话快答）
    ├── overview.md               # 能力集概览：覆盖范围、能力衔接、限制与不覆盖
    └── glossary.md               # 术语表（本能力集内的定义）
```

## 用法

1. 先读 `SKILL.md`，按意图路由表加载 **1** 张能力卡（跨域任务最多 2 张）。
2. 卡内 E 段就是执行清单：照做即可，产出物（名单、脚本、台账、诊断表）都由你自己填。
3. 快答查 `cheatsheet.md`，术语查 `glossary.md`，边界与覆盖问题查 `overview.md`，
   路由表命中不了的意图查 `capability-index.md`。
4. 卡内出现"本卡推断"时，说明该判据是使用者约定：首次使用请把自己的阈值写下来。

## 不适用

- 薪酬数字、市场区间与报价（包内不含定价数据）。
- 劳动法、仲裁、遣散与竞业条款的法律解释。
- 临床心理议题（社交焦虑症、惊恐、抑郁）。
- 需要当期统计或政策依据的问题：本能力集的时效基线约二十年前，且不随包更新。

## 18 项能力

| 簇 | 能力 |
|---|---|
| 沟通 | prewire-disagreement（会前预连线与异议表达）· meeting-voice（会议发言争取）· upward-dialogue（向上沟通：澄清/改判/说不）· nonverbal-credibility（眼神与可信度）· behavior-reframe（双刃行为转换器） |
| 晋升 | win-file（成果归档）· performance-discussion（绩效谈话与全年反馈）· comp-negotiation（薪酬与晋升谈判准备）· guide-map（引导者四型地图）· mobility-audit（天花板与流动性诊断）· new-role-infrastructure（新岗位 90 天） |
| 求职 | role-targeting（岗位定位）· pitch-three-s（个人说辞三约束）· interview-narrative（面试成就叙述重写）· interview-rehearsal（面试演练闭环）· network-long-game（人脉分层与长期维护）· employer-fit-probe（雇主适配尽调）· external-feedback-probe（外部反馈征集） |
