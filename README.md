# Curriculum Development Loop

面向 Agent 技术培训的课程开发闭环 Skill：共同选题、框架评审、资料调研、教学样章、课件开发、试讲与持续迭代。

## 项目状态

当前为 v0.4.0 工作流规范，尚未经过完整真实课程试跑或目标学员效果验证。项目仓库为 [wang123good/Curriculum-Development-Loop](https://github.com/wang123good/Curriculum-Development-Loop)，通过 Git 同步 Skill 与配套文档。

## 适用对象与约束

- 学员具有 1～3 年软件研发或算法开发经验。
- 每课课件阅读目标为 30～40 分钟，定位时确认纯阅读或完整核心学习口径；思考、视频、Demo 操作、等待和试讲分别记录。未确认时按纯阅读估算。
- 内容需要覆盖技术机制、具体示例、工程取舍与适用边界。
- 每课应与既有课程形成知识依赖和前后呼应。
- 选题、框架、教学样章及最终试讲验收由课程负责人参与评审。

## 工作流

共同选题 → 框架讨论与评审 → 高价值资料调研 → 教学样章评审 → 完整开发 → 阅读走查与试讲 → 修订验收 → 课程与流程复盘。

评审可以返回相关阶段。网页教材、PDF 教材、概念视频及 Demo 分别可选，不作为课程默认必备交付物。

## 使用方式

将 `skills/curriculum-development-loop` 文件夹复制到所用 Agent 支持的 Skill 目录，或让 Agent 读取其中的 `SKILL.md`。本项目不附带自动发布或自动同步程序。

示例请求：

> 使用 curriculum-development-loop，与我讨论一节 Agent 工具调用课程的选题。先评审主题范围和前课衔接，不进入课件制作。

> 继续当前课程，根据试讲意见修改解释和展示方式，并记录本次课程变更与工作流改进建议。

## 文件结构

```text
README.md
CHANGELOG.md
.gitignore
skills/
  curriculum-development-loop/
    SKILL.md
    references/
      workflow.md
      provenance.md
      operations.md
      quality.md
    assets/
      course-records.md
```

## 开发与评审约定

调整工作流时记录修改原因、适用范围及影响阶段；单课偏好不自动成为永久规则。保持 Skill 入口简洁，将详细方法放在参考文件中。提交变更前检查文件链接、可选交付项、评审节点及时间约束的一致性。

课程项目应分别维护课程任务书、资料来源、进度与决策、评审问题和版本记录。修改概念后检查所有已启用载体的关联内容。

## 执行机制

- 用 `course-state.md` 作为课程进度唯一入口，恢复任务时核对实际成果。
- 阶段交接有最低产物与通过条件，评审绑定成果版本，重大改动触发相关重审。
- 系列地图管理能力依赖；稳定教学单元 ID 连接底稿与各载体。
- 试讲区分模拟、负责人评审和真实学员验证；各交付物分别验收。
- 每轮区分必修项、优化项和后续增强，明确收尾条件。
- 进行中的课程绑定工作流版本，升级需评估影响并由负责人决定。
- 默认一个主 Agent 负责整合，按需调用制作能力；不默认启动多 Agent。
- 用户指令与闭环规范冲突时，主动说明规则来源、缺口、影响和最小调整；用户可明确决定本课例外或长期修订，决定需记录，不静默跳过评审。
- 启动课件开发时先提交主题理解卡；主题确认后逐项记录交付物意向，框架阶段再锁定 PDF、网页、动画、教学案例、Demo 或示例代码的最终范围。
- 技术教学检查覆盖核心解释链、机制完整性、简单基线、原理到实现映射和课件独立阅读，嵌入现有评审节点。
- 轻量检查岗位价值、适学人群、总学习投入和代表性达标任务；复盘区分交付质量、学习效果与岗位应用证据，不强制新增考试或审批。

使用 [课程记录模板](skills/curriculum-development-loop/assets/course-records.md) 按需建立记录。详细交接见 [状态规范](skills/curriculum-development-loop/references/operations.md)，试讲与产物验收见 [质量规范](skills/curriculum-development-loop/references/quality.md)。模板不包含已完成课程或试跑证据；首门课程选题确定后再执行真实闭环。

## 来源与许可

本项目以本次课程设计讨论为基础，参考公开教学设计 Skill 的方法并重新组织，来源及核实范围见 [参考说明](skills/curriculum-development-loop/references/provenance.md)。未复制第三方程序或整份 Skill。当前未授予开源许可；任何第三方材料仍适用其原有许可。
