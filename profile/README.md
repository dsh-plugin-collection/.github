# DSH plugin collection

本组织维护 [DeepSeek Harness](https://github.com/deepseek-ai/DeepSeek-Harness) 的插件。

## 设计原则

- **不喧宾夺主**：像 DSH 原生能力一样自然，不抢宿主的存在感。
    - 优先复用官方图标集与 UI 原语、跟随官方样式与主题、注入官方挂载点，而非自带一套。
    - 尽量不占显眼或高频位置，不打断主流程，不反复强调自身。
    - 优先扩展而非替换官方既有行为。
- **不过度设计**：优先最克制、够用的方案，能少一层抽象就少一层。
- **配置自由**：关键行为尽量可配置，把选择权交给用户。
- **不重复造轮子**：优先复用官方能力、已有插件和成熟依赖，不另起等价实现。
- **性能保证**：尽量不阻塞主线程、不做无谓重排与轮询，不给宿主添负担。
- **足量测试**：关键路径尽量有测试覆盖，升级不悄悄破坏既有行为。

## 插件

| | 插件 | 版本 | 说明 |
| --- | --- | --- | --- |
| <img src="https://raw.githubusercontent.com/dsh-plugin-collection/dsh-later/main/icon.svg" width="24"> | [dsh-later](https://github.com/dsh-plugin-collection/dsh-later) | ![npm](https://img.shields.io/npm/v/dsh-later) | 给 DSH 加上定时发送：输入一句话，到点自动以你的身份送出，关掉网页也准时触发。 |
| <img src="https://raw.githubusercontent.com/dsh-plugin-collection/dsh-suggest-ghost/main/icon.svg" width="24"> | [dsh-suggest-ghost](https://github.com/dsh-plugin-collection/dsh-suggest-ghost) | ![npm](https://img.shields.io/npm/v/dsh-suggest-ghost) | 给 DSH 输入框加上输入预测：回合结束后自动建议你的下一句话，Tab 一键采纳。 |
| <img src="https://raw.githubusercontent.com/dsh-plugin-collection/dsh-group-status/main/icon.svg" width="24"> | [dsh-group-status](https://github.com/dsh-plugin-collection/dsh-group-status) | ![npm](https://img.shields.io/npm/v/dsh-group-status) | DSH 侧栏折叠分组聚合徽标：收起的文件夹行显示聚合状态，带数字与悬停明细。 |
| <img src="https://raw.githubusercontent.com/dsh-plugin-collection/dsh-herdr-site/main/icon.svg" width="24"> | [dsh-herdr-site](https://github.com/dsh-plugin-collection/dsh-herdr-site) | ![npm](https://img.shields.io/npm/v/dsh-herdr-site) | 让 Herdr 认识 DSH 面板：把 agent 的 working/idle/blocked 状态报给 Herdr。 |

说明摘自各插件的 `package.json`；版本由 shields.io 实时读取 npm，无需手动同步。

## 安装

```bash
dsh plugin install dsh-later
dsh plugin install dsh-suggest-ghost
dsh plugin install dsh-group-status
dsh plugin install dsh-herdr-site
```
