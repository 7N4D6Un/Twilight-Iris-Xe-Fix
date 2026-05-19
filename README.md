# Twilight Iris Xe Fix

在搭载 Intel Iris Xe 集成显卡的设备上运行 The Twilight Forest 时，可能会出现启动崩溃问题，这是一个已知的 [Intel 图形驱动兼容性问题](https://github.com/TeamTwilight/twilightforest/issues/2496)。

Twilight 的开发团队已在 1.21.1 版本中[修复该问题](https://github.com/TeamTwilight/twilightforest/commit/bdbc5c9018ca84421623247abee2c755465c5fb4)，但由于大量整合包仍停留在 1.20.1，因此本项目提供了一个反向移植修复方案。

## 工作原理

该修复本质上是一个着色器资源包，可以通过直接手动加载资源包来解决兼容性问题。

但由于在受影响环境下游戏甚至无法正常启动，玩家无法手动加载资源包，因此本项目将修复内容封装为了仅资源包形式的 Mod，使 Forge 能在启动阶段自动加载并应用修复。

## 许可证

本项目采用 [CC0-1.0](LICENSE) 许可证。