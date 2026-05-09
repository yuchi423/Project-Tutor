---
name: tutorbegin
description: initiallized the memory, launching the program-tutor
disable-model-invocation: false
---
### 1. `/tutorbegin -Welcome and Meet the Learner`
- **执行步骤**：
  1. **环境检测**：检查当前工作目录下是否存在 `docs/tutor_memory.md` & `docs/process-notes.md` 文件。
  
  2. **分支 A：恢复进度模式 (记忆文件已存在)**
     - **深度读档**：自动读取 `docs/tutor_memory.md` 与 `docs/process-notes.md`。
     - **状态分析**：在任务树中定位当前第一个状态为 `[ ] 未完成` 的 Task，并扫描 `process-notes.md` 中学生最近的决策和挣扎点。
     - **暖场与复盘**：在对话中输出简短的欢迎语。总结已完成的进度，并巧妙地提及上次的难点或决策（例如：“欢迎回来！根据记录，我们已经完成了基础数据结构，上次你在处理指针越界时展现了很好的 Debug 思路。”）。
     - **无缝衔接**：直接将学生带回当前未完成 Task 的工作流中（根据上下文判断是继续 Phase 2 的 Unlock 提问，还是继续检查 Phase 3 的代码）。**绝对不要**重新输出完整的蓝图或重新初始化文件。

  3. **分支 B：首次初始化模式 (记忆文件不存在)**
    阅读project/project_requirements.md ，了解项目背景和需求。
    阅读skills/program-guide.md，熟悉项目导师的核心知识和行为规范,then follow this command。
    - **触发动作**：初始化项目。
    - **执行步骤**：
  1. 分析项目说明，将项目拆解为多个 Milestone，每个 Milestone 包含具体的 Tasks。
  2. 创建docs文件夹，之后的md文档都保存在这里，例如 `tutor_memory.md`、`process-notes.md` 等。
  3. 自动在当前工作目录下创建或覆写 `tutor_memory.md` 文件与` process-notes.md` 。
  4. 将完整的任务蓝图（状态设为 `[ ] 未完成`）和关键设定写入 `tutor_memory.md`。
  5. 在对话中输出任务蓝图，并直接进入 Milestone 1 的 Task 1 的 **Phase 2 (Unlock)** 阶段。

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