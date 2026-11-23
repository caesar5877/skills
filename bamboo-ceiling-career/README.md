# bamboo-ceiling-career

Agent Skill：把 Jane Hyun《Breaking the Bamboo Ceiling》蒸馏成**可执行的能力卡**，覆盖三簇场景 ——
**沟通**（会议发言 / 表达异议 / 向上沟通）、**晋升**（成果归档 / 绩效讨论 / 导师与成长机会）、
**求职**（岗位定位 / 面试表达 / 人脉交流）。

- 格式：`SKILL.md` 入口 + `references/capabilities/*.md` 能力卡（single 模式，1 个可发现入口）
- 蒸馏工具：[cangjie-skill v2.5.0](https://github.com/kangarooking/cangjie-skill)（RIA-TV++ 七阶段流水线）
- 校验：`validate_skill_pack.py` → 0 errors / 0 warnings

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
    ├── cheatsheet.md             # 决策规则速查（不含原文依据的快答）
    ├── overview.md               # 整书概览（回答"这本书讲了什么"）
    └── glossary.md               # 术语表（作者的特定用法）
```

## 18 项能力

| 簇 | 能力 |
|---|---|
| 沟通 | prewire-disagreement（会前预连线与异议表达）· meeting-voice（会议发言争取）· upward-dialogue（向上沟通：澄清/改判/说不）· nonverbal-credibility（眼神与可信度）· behavior-reframe（双刃行为转换器） |
| 晋升 | win-file（成果归档）· performance-discussion（绩效谈话与全年反馈）· comp-negotiation（薪酬与晋升谈判准备）· guide-map（引导者四型地图）· mobility-audit（天花板与流动性诊断）· new-role-infrastructure（新岗位 90 天） |
| 求职 | role-targeting（岗位定位）· pitch-three-s（三 S 个人说辞）· interview-narrative（面试成就叙述重写）· interview-rehearsal（面试演练闭环）· network-long-game（人脉分层与长期维护）· employer-fit-probe（雇主适配尽调）· external-feedback-probe（外部反馈征集） |

## 硬边界（入口已写入，卡内亦有）

- **不提供薪酬数字、市场区间或报价建议**：源书不含薪酬数据，且基线为 2005 年美国市场。
  本技能交付的是谈判的结构（区间 / 愿望清单 / 下限三要素与组件化拆解），数据须由使用者接当期来源。
- **不提供法律结论**：劳动法、仲裁、遣散与竞业条款超出范围（原书为美国雇佣语境）。
- **不处理临床议题**：社交焦虑、自闭谱系等应转专业支持；原书框架假定非临床人群。
- **不做群体画像**：族裔相关概念描述的是特定制度的机制，不得用于预测或评判具体个人。
- **时效**：书内统计截至 2004 年，职场场景为 2005 年前后（无 LinkedIn、无远程面试）；
  各卡 `B` 段已逐条标注需要重新校准之处。

## 来源与版权说明

- 本包为对 Jane Hyun《Breaking the Bamboo Ceiling》（2005, Berrett-Koehler）的**摘要与分析性归纳**，
  **不包含该书文字**：全部卡文为原创改写，引用限于术语级短语与页码定位。
  发布前已做逐字重叠检测（以 12 词连续片段为阈值比对全书 98,390 词）：**命中 0 处**。
- 书中两个测评工具（Seven Stories / Forty-Year Vision）为第三方授权内容，
  本包仅重述其方法、未复制量表条目。
- 与原作者、出版社及 cangjie-skill 项目无隶属关系。
- 技能骨架沿用 cangjie-skill 的 MIT 许可；本目录内的摘要文字无额外授权限制。

## 已知局限（发布时如实声明）

1. **未逐页通读原书**：按上述三簇做定向全量扫描；原书部分章节（文化根源散文、家庭协商、
   专业协会运作细节、组织名录附录）未纳入能力，已判定为背景或过期参考。
2. **一处原文表格未完全校验**：原书"行为→误读→资产"对照表在 PDF 文本层列序粘连，
   相关卡的四列结构与已核读行可靠，逐格值需回看原书表格页。
3. **评测为自评自跑**：触发评测与输出评测由蒸馏者本人执行（无独立 sub-agent），
   结果仅可作回归基线，不构成独立效度证明。

## 建议用法

先让入口路由，再按需加载 1 张卡；概览类问题只读 `references/overview.md` 与入口的核心原则。
不要一次加载多张卡——卡与卡之间有 `also_read` 指针，按任务追加即可。
