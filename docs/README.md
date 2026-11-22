# 面试练习室项目知识库

开工先看下表。从前往后，先选一张前置任务已经验收的票，然后只读它对应的设计章节。

| 顺序 | 开发任务 | 开工前读 | 这一步交付什么 |
| --- | --- | --- | --- |
| 1 | [#2 总结定位与专项复练](https://github.com/kris-builder/ai-interview/issues/2) | [总结到复练](architecture/interview-review.md#阶段一总结到复练) | 从薄弱点找到对应原答，进入变式或回看已有对照。 |
| 2 | [#3 对照评估](https://github.com/kris-builder/ai-interview/issues/3) | [按各自题意对照](architecture/interview-review.md#阶段二按各自题意对照) | 用原题与变式的真实条件判断用户补上了什么。 |
| 3 | [#4 单轮复盘持久化](https://github.com/kris-builder/ai-interview/issues/4) | [稳定回看](architecture/interview-review.md#阶段三稳定回看) | 同一原答的点评与练习可在刷新后稳定回看。 |

父规格和任务状态在 [GitHub Issue #1](https://github.com/kris-builder/ai-interview/issues/1)。任务的阻塞关系、进度、验收勾选和本次测试结果在对应 Issue 维护。

## 什么时候读哪份文档

| 需要回答的问题 | 文档 |
| --- | --- |
| 用户要走完什么流程，哪些行为已经确认？ | [面试与复练产品规格](product/interview-practice.md) |
| 该改哪个模块、数据从哪来、怎么验？ | [复盘架构与技术设计](architecture/interview-review.md) |
| 这个方案为什么这样定，哪些旧方案已经退役？ | [历史决策](decisions.md) |

## 使用 to-spec 和 to-tickets

1. **用 `to-spec` 确认规格。** 把确认后的用户行为及范围写入对应产品规格。涉及模块职责、数据归属或交互约定时，同步补充技术设计。影响后续取舍的决定写进历史决策。双向链接本地文档与规格 Issue。
2. **用 `to-tickets` 拆开发任务。** 每次都在对应技术设计补充或核对可复用的内容，包括分阶段的模块改动、迁移顺序和验收方法。用链接指向任务 Issue。若多个任务共用同一设计，维护一份主题文档即可。
3. **开发和验收。** 开工时看当前票的验收目标，改动时查模块边界，验收后把实际结果和待复测项写回该票。设计变化时更新原有章节。已被替换的决策保留经过，并注明后续采用的方案。
4. **同步。** 本地 Markdown 随 Git 提交同步到 GitHub。跨分支审阅可从规格 Issue 提供的 PR 链接进入，合入后用默认分支的文档链接。
