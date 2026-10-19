# 贡献指南

本组织维护 [DeepSeek Harness](https://github.com/deepseek-ai/DeepSeek-Harness) 的插件。欢迎提 Issue 报问题、提 PR 改进。

## 设计原则

以下原则是本组织所有插件的准绳（与组织主页同源，改其一须同步另一）：

- **不喧宾夺主**：像 DSH 原生能力一样自然，不抢宿主的存在感。
    - 优先复用官方图标集与 UI 原语、跟随官方样式与主题、注入官方挂载点，而非自带一套。
    - 尽量不占显眼或高频位置，不打断主流程，不反复强调自身。
    - 优先扩展而非替换官方既有行为。
- **不过度设计**：优先最克制、够用的方案，能少一层抽象就少一层。
- **配置自由**：关键行为尽量可配置，把选择权交给用户。
- **不重复造轮子**：优先复用官方能力、已有插件和成熟依赖，不另起等价实现。
- **性能保证**：尽量不阻塞主线程、不做无谓重排与轮询，不给宿主添负担。
- **足量测试**：关键路径尽量有测试覆盖，升级不悄悄破坏既有行为。

## 开发

- 各插件的本地构建与运行方式见其仓库 README。
- 新增用户可见文案优先走官方 locale（`@deepseek-ai/dsh-client-locale`），不硬编码。
- UI 优先复用官方图标集与 UI 原语（`@deepseek-ai/dsh-client-ui-primitives`）。

## 发布

版本发布与推送（npm、GitHub/Gitea、catalog 收录三方一致）遵循 `RELEASE-OPS.md`。

## 收录到插件市场

向 `awesome-dsh-plugin` 提交收录，要求见其 `contributing.md`（`dsh.bundle` manifest、真实代码、活跃维护、`dsh-plugin` topic、描述无营销词）。
