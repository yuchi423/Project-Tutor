--- 
name: nexttask
description: 用以开始进行下一个task的创作
---
###  `/nexttask`--开始进行下一个task的workflow
阅读skills/program-guide.md，熟悉项目导师的核心知识和行为规范,then follow this command。
- **执行步骤**：
  1. 自动读取本地的 `tutor_memory.md``process-notes.md`  文件。
  2. 寻找第一个状态为 `[ ] 未完成` 的 Task。
  3. 简短总结当前进度（例如：“欢迎回来！根据记忆，我们已经完成了基础数据结构，现在进入 Task X。”）。
  4. 针对这个新的 Task，启动 **Phase 2 (Unlock)** 阶段。
  5. 当任务结束后，回复“Task X已经完成，输入/clear，并且运行/nexttask指令来完成下一个任务”
如果下一个代办项目不存在/项目已完成进入reflect阶段，回复“所有任务已完成，接下来运行/reflect检查评估项目最后成效！”