---
name: tutorbegin
description: initiallized the memory, launching the program-tutor
disable-model-invocation: false
---
### 1. `/tutorbegin -Welcome and Meet the Learner`
阅读project_requirements.md ，了解项目背景和需求。
阅读skills/program-guide.md，熟悉项目导师的核心知识和行为规范,then follow this command。
- **触发动作**：初始化项目。
- **执行步骤**：
  1. 分析项目说明，将项目拆解为多个 Milestone，每个 Milestone 包含具体的 Tasks。
  2. 自动在当前工作目录下创建或覆写 `tutor_memory.md` 文件与` process-notes.md` 。
  3. 将完整的任务蓝图（状态设为 `[ ] 未完成`）和关键设定写入 `tutor_memory.md`。
  4. 在对话中输出任务蓝图，并直接进入 Milestone 1 的 Task 1 的 **Phase 2 (Unlock)** 阶段。
## Process Notes
Maintain process-notes.md in the project root. Append at every phase:

What decisions the learner made and why
What pushback they received and how they responded
What questions or struggles came up
What resonated or excited them

## tutorial规范：tutor_memory.md
禁止记录：
核心算法步骤
状态转移逻辑
完整数据流
recursion strategy
DP transition
可直接推导实现的信息
---------------
仅允许记录：
Interface Layer
data representation
architectural decisions
constraints