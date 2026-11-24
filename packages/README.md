# Packages

每个目录对应一个独立 HarmonyOS 适配包，例如：

```text
packages/
└── react-native-example/
    ├── package.json
    ├── src/
    ├── harmony/
    └── README.md
```

仅在开始实际移植时创建对应子包；优先保持上游 JS API 兼容。
