# Project萤

ProjectYing 是 AITermux 的终端 AI 工作台，面向 Android + Termux 环境开发。

## 状态

ProjectYing 仍处于实验性测试阶段，请勿用于日常生产或长期稳定使用。当前版本只具备研究、验证和测试价值。

我们会尽最大努力降低它的使用门槛，但它仍然会保持较高难度。使用者需要理解 Termux、API Key、模型代理、文件权限、终端日志，以及工具调用带来的系统风险。

## 适用范围

- AITermux / Termux 环境
- Android 设备上的终端 AI 工作流测试
- 多 Agent 协同、上下文治理、工具调用、手机自动化等实验性能力验证

ProjectYing 不是通用桌面程序，不承诺支持 Linux 桌面、Windows、macOS 或普通 Android shell。

## 当前边界

- 基于第三方 Codex API 链路，暂未适配其它 API。
- 当前主要面向中转站 Codex 使用。
- 发布仓库只提供源码与空白初始化模板。
- 不包含任何 API Key、聊天历史、memory、上下文、Aidebug 运行日志或 target 构建产物。

## 实验能力

- Matrix 母体 Agent 调度
- 多 Agent 协同与子 Agent 调度
- 永久记忆、fastmemory 与多层压缩机制
- 动态上下文、专注模式交叉上下文与上下文治理工程
- AIdebug 智能系统
- 编程、服务器运维与终端工具调用
- TERMUX 终端触控
- 对账策略系统与升级蓝图计划工具
- Agent 自优化与 Matrix 自生长实验

## 入门门槛

- Android + Termux
- 已安装 AITermux
- 基础 Linux / Termux 使用能力
- 能理解 API Key、模型代理、文件权限和终端日志
- 具备基础计算机、AI 与 Agent 概念
- 部分手机自动化、ADB、服务器管理能力可能需要额外授权、无线调试或 root 环境

## 启动

通常由 AITermux 启动器拉起：

```bash
cd ~/AItermux/projectying
./run.sh
```

首次启动会在本地生成运行配置、上下文、记忆和日志。不要把这些运行态文件提交到仓库。

## 构建

```bash
pkg install rust clang make pkg-config
cargo build --release
```

## 使用前确认

- 只在 AITermux / Termux 链路内使用。
- 使用前先阅读源码和配置，确认你知道它会调用哪些工具。
- 不建议普通用户在不了解 Termux 文件结构、权限和模型 API 风险的情况下直接使用。
