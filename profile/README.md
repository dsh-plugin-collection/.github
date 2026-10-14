# DSH Plugin Collection

DSH (DeepSeek Harness) 插件集合。本组织维护为 DSH 开发的各类插件。

## 插件列表

| 插件 | 描述 | 状态 |
| --- | --- | --- |
| [dsh-later](https://github.com/dsh-plugin-collection/dsh-later) | 会话内定时消息调度，支持智能时段建议和待发送管理 | 稳定 |
| [dsh-suggest-ghost](https://github.com/dsh-plugin-collection/dsh-suggest-ghost) | 输入预测插件，LLM 生成下一条建议，幽灵文本渲染 | 稳定 |
| [dsh-group-status](https://github.com/dsh-plugin-collection/dsh-group-status) | 多会话状态管理，树形结构展示会话组状态 | Beta |
| [dsh-herdr-site](https://github.com/dsh-plugin-collection/dsh-herdr-site) | Herdr 终端工作区集成，上报 agent 状态 | 稳定 |

## 插件分类

```
┌─────────────────────────────────────────────────────────────┐
│  核心功能          │  智能增强          │  集成扩展          │
│  dsh-later         │  dsh-suggest-ghost │  dsh-herdr-site    │
│  dsh-group-status  │                    │                    │
└─────────────────────────────────────────────────────────────┘
```

## 安装

通过 DSH 插件市场搜索并安装，或使用命令行：

```bash
dsh plugin install dsh-later
dsh plugin install dsh-suggest-ghost
dsh plugin install dsh-group-status
dsh plugin install dsh-herdr-site
```

## 贡献

欢迎提交 Issue 报告问题，或提交 PR 修复问题、添加新特性。

## 维护

由 [WuJiaoJue](https://github.com/WuJiaoJue) 维护。

基于 [DeepSeek Harness](https://github.com/deepseek-ai/DeepSeek-Harness)。
