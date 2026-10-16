# Curriculum Development Loop

面向 Agent 技术培训的课程开发闭环 Skill：共同选题、框架评审、资料调研、教学样章、课件开发、试讲与持续迭代。

## 项目状态

当前为 v0.1 工作流讨论草案，尚未经过完整课程试跑。项目仓库为 [wang123good/Curriculum-Development-Loop](https://github.com/wang123good/Curriculum-Development-Loop)，通过 Git 同步 Skill 与配套文档。

## 适用对象与约束

- 学员具有 1～3 年软件研发或算法开发经验。
- 每课核心阅读及必学媒体合计预计 30～40 分钟，实际时间由阅读走查校准；现场试讲时间另行记录。
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
```

## 开发与评审约定

调整工作流时记录修改原因、适用范围及影响阶段；单课偏好不自动成为永久规则。保持 Skill 入口简洁，将详细方法放在参考文件中。提交变更前检查文件链接、可选交付项、评审节点及时间约束的一致性。

课程项目应分别维护课程任务书、资料来源、进度与决策、评审问题和版本记录。修改概念后检查所有已启用载体的关联内容。

## 来源与许可

本项目以本次课程设计讨论为基础，参考公开教学设计 Skill 的方法并重新组织，来源及核实范围见 [参考说明](skills/curriculum-development-loop/references/provenance.md)。未复制第三方程序或整份 Skill。当前未授予开源许可；任何第三方材料仍适用其原有许可。
