# rnoh-ports

React Native OpenHarmony ports and native adaptations.

用于集中维护 React Native 第三方库的 HarmonyOS（RNOH）移植与原生适配实现。

## 目录

```text
rnoh-ports/
├── packages/           # 每个可独立发布的 RNOH 适配包
├── apps/               # 示例与调试应用（按需添加）
├── docs/               # 兼容性、架构和移植记录
├── package.json
└── pnpm-workspace.yaml
```

## 开发原则

- 每个移植库独立维护 `package.json`、源码、测试和说明。
- 保持 React Native 上游 JS API 兼容；Harmony 原生实现放在子包的 `harmony/` 目录。
- 按实际需要增加子包，不预创建未实现的第三方库。
- 使用 pnpm workspace 管理多包；发布策略与包名在第一个适配包落地时确定。

## 开始

```bash
corepack enable
pnpm install
```

> 当前仅包含 Monorepo 根配置，尚未添加具体适配包或 HarmonyOS 示例工程。
