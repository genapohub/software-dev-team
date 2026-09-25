# 复合一体化产品团队 — mvp-expert-team

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-2.0.0-green.svg)](SKILL.md)

一个面向 AI 编程助手的 **复合一体化产品团队 Skill**——项目总监统筹 7 位领域专家（产品经理 / 首席架构师 / UI设计师 / 前端工程师 / 后端工程师 / 测试工程师 / 运维工程师）。**既能从一句话想法做 MVP 快速开发与原型验证（端到端交付可运行可部署产品），又能持续做产品迭代、功能扩展与工程维护（增量开发 / 缺陷修复 / 灰度发布 / 长期运维）。** 阶段门禁 + 团队级 P0 反 AI 规则，自包含、不依赖任何其他 Skill。

> 2026-09-25 融合 WorkBuddy「软件开发团队 software-company」专家，在原 MVP 专家团基础上补齐「MVP 交付不是终点」的迭代维护闭环。详见 `references/expert-distill/software-company-蒸馏.md`。

## 能力

- **双轨流水线**：Track A（MVP 从零交付：需求澄清 → 调研 → Spec → 设计 → 开发 → 测试 → 部署）+ Track B（产品迭代与工程维护：现状评估 → 增量定义 → 增量设计 → 增量开发 → 回归+智能路由 → 发布运维）+ Track C（BugFix）+ Track D（部分工作流）
- **生命周期闭环**：MVP 跑起来 → 试运营反馈 → 持续迭代 → 工程维护 → 大版本重构回 Track A，同一个团队两种节奏
- **团队级 P0 三红线**：禁 emoji 作功能图标 / 禁紫→粉渐变主视觉 / 禁 AI 模板味（空洞占位、硬编码色、千篇一律 Hero）——每道门禁强制执行
- **机器可读契约**：openapi.yaml + design-tokens.json 作为放行门槛，反 AI 味从设计层落到代码层
- **测试反作弊门 + 智能路由**：先写测试（写测试的 ≠ 写代码的）+ 5 类作弊检测 + P0 缺陷归零才上线；迭代期智能路由裁决（源码 bug→工程 / 测试 bug→自修 / 全过→NoOne，≤2 轮封顶）
- **增量开发纪律**：既有代码上最小变更、保留既有行为、回归率=0，拒绝"凭空重写"
- **两种执行模式**：多代理编排（子代理并行）/ 单代理角色切换（换视角自审），产出与门禁一致

## 团队构成（自包含 7 角色）

| 角色 | 文件 | 职责 |
|------|------|------|
| 产品经理 | `agents/01-产品经理-pm.md` | 需求挖掘、竞品调研（差评找空白）、RICE 排序、PRD |
| 首席架构师 | `agents/02-首席架构师-architect.md` | 技术选型对比矩阵、API/DB 契约、ADR、可行性验证 |
| UI设计师 | `agents/03-UI设计师-designer.md` | 寄存器判断、反 AI 模板主职、四层 Token、DESIGN.md |
| 前端工程师 | `agents/04-前端工程师-frontend.md` | 设计不过反模式检查不写代码、自检循环、19 项视觉检查 |
| 后端工程师 | `agents/05-后端工程师-backend.md` | 分层架构、错误三层、安全清单、失效模式 6 类自检 |
| 测试工程师 | `agents/06-测试工程师-qa.md` | 先写测试、反作弊门、回归集沉淀、生产就绪评级 |
| 运维工程师 | `agents/07-运维工程师-devops.md` | 部署可回滚、健康检查、备份、自包含交付包 |

> 7 位专家**均具备 MVP 从零 + 迭代维护双重能力**——每位角色文件末尾均有「迭代与维护（持续交付职责）」段落。

## 触发热词

做成MVP、从零开发、一句话变产品、帮我做个产品、端到端交付、全栈实现、需求到上线、完整产品开发、MVP开发、加功能、改bug、迭代、维护、续作、持续优化、上线后、产品迭代

---

## 安装

本 Skill 遵循 **Open Agent Skills 标准**（SKILL.md 格式），兼容以下工具：

### WorkBuddy / CodeBuddy

**方式一：克隆到 skills 目录**
```bash
git clone https://github.com/genapohub/mvp-expert-team.git ~/.workbuddy/skills/mvp-expert-team
```

**方式二：ZIP导入**
```bash
git clone https://github.com/genapohub/mvp-expert-team.git
zip -r mvp-expert-team.zip mvp-expert-team/
```
然后在 WorkBuddy 桌面端 → **技能市场** → **添加技能/上传技能** → **点击"跳过检测，直接安装"**。

### Trae

**ZIP 导入**
```bash
git clone https://github.com/genapohub/mvp-expert-team.git
```
然后在 Trae → **设置** → **Rules & Skills** → **创建** → 上传 `mvp-expert-team.zip`。

### Codex / ZCode

```bash
# 克隆到 skills 目录
git clone https://github.com/genapohub/mvp-expert-team.git ~/.codex/skills/mvp-expert-team

# ZCode
git clone https://github.com/genapohub/mvp-expert-team.git ~/.zcode/skills/mvp-expert-team
```

重启 Codex / ZCode 客户端后自动发现。也可以在对话中输入 `$mvp-expert-team` 手动调用。

### Cursor
```bash
# 克隆到 skills 目录
git clone https://github.com/genapohub/mvp-expert-team.git ~/.cursor/skills-cursor/mvp-expert-team
```

重启 Cursor客户端 后自动发现。也可以在对话中输入 `$mvp-expert-team` 手动调用。

---

## 仓库结构

```
mvp-expert-team/
├── SKILL.md                     # 项目总监主控：定位/P0红线/快速路径/执行模式/6阶段/角色索引/门禁
├── README.md                    # 本文件
├── LICENSE                      # MIT
├── .gitignore
├── agents/                      # 7 个角色独立文件（各含完整方法论与模板）
│   ├── 01-产品经理-pm.md
│   ├── 02-首席架构师-architect.md
│   ├── 03-UI设计师-designer.md
│   ├── 04-前端工程师-frontend.md
│   ├── 05-后端工程师-backend.md
│   ├── 06-测试工程师-qa.md
│   └── 07-运维工程师-devops.md
├── memory/                      # 技能记忆区（每次调用先读后写，随技能携带）
│   ├── README.md                # 记忆目录说明
│   ├── MEMORY.md                # 长期记忆：可复用决策/用户偏好
│   ├── project-tracker.md       # 项目进度台账：里程碑/裁决
│   ├── YYYY-MM-DD.md            # 活跃日志（运行时追加）
│   └── archive/                 # 月度归档
└── references/                  # 团队共享知识库
    ├── 01-全流程模板库.md       # PRD/Spec/OpenAPI/ADR/DESIGN/质量报告/增量卡等可填空模板
    ├── 02-P0规则与反AI清单.md   # 红线细规 + 7大罪 + 12禁令 + 19项视觉检查 + AI痕迹检测
    ├── 03-工程纪律与自检.md     # 代码组织/失效模式6类/测试反作弊/记分卡/门禁汇总
    ├── 04-记忆规则.md           # memory/ 生命周期：读写时机/日志格式/轮转归档算法
    ├── 05-产品迭代与工程维护.md # Track B 纵深方法论：增量开发/缺陷修复/灰度发布/长期运维
    └── expert-distill/          # 专家蒸馏溯源
        └── software-company-蒸馏.md  # 软件开发团队专家蒸馏（角色/职责/能力边界/可复用增量）
```

## 使用

**触发**：说出想法或迭代诉求 → 自动以项目总监身份启动 → 路由到对应轨道

```
[一句话想法]            [既有项目 + 迭代/缺陷/维护诉求]
    ↓ Track A                ↓ Track B
Phase 0 需求澄清      I-0 现状评估（读 Spec+代码+记忆）
    ↓                     ↓
Phase 1 并行调研      I-1 增量需求卡 → I-2 增量设计
    ↓ 【确认三文档】         ↓ 【不破坏既有契约】
Phase 1.5 Spec 锁定   I-3 增量开发（最小变更）
    ↓                     ↓
Phase 2 设计细化      I-4 回归+智能路由（≤2轮）
    ↓ 【P0+反模式+契约】      ↓ 【P0 归零+反作弊+回归率0】
Phase 3 并行开发      I-5 发布+运维长跑（灰度/监控/回滚）
    ↓ 【代码组织+emoji+视觉】
Phase 4 测试交付（P0 归零 → 部署 → 交付包）
    ↓
[可运行 MVP 或 增量交付 + 自包含交付包 + 7×3 评级 ≥ Silver]
```

**使用示例**：

```
我想从零做一个团队协作工具，做成 MVP        # → Track A
帮我开发一个电商小程序                    # → Track A
给宠宝树后台加个 AI 客服模块              # → Track B 功能扩展
列表分页少了一页，修一下                  # → Track C BugFix
给已上线项目做下性能优化                   # → Track B 工程维护
```

主控按工作流路由总表（轻量/标准/迷你/Track B/Track C/部分）判定轨道，逐 Phase 门禁推进。

## 来源与致谢

本技能承载 WorkBuddy「MVP开发专家团」专家包 v2.1.0（大湾区靓仔 × 7 专家团队）的完整方法论，2026-09-06 整理为独立技能；2026-09-25 融合 WorkBuddy「软件开发团队 software-company」专家，补齐增量开发 / 缺陷修复 / 测试智能路由 / 产品生命周期闭环，升级为复合一体化产品团队 v2.0.0。工程纪律部分源自该专家包内嵌的 UmaDev 知识库方法论（MIT License，详见 `references/03-工程纪律与自检.md`）。内容剔除多 Agent 环境专属机制（Team spawn / SendMessage / IMA MCP），适配多代理与单代理两种执行模式。融合溯源见 `references/expert-distill/software-company-蒸馏.md`。

## 许可

[MIT](LICENSE) © zhangmengbo
