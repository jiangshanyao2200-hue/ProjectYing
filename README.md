# Project萤

ProjectYing 是 AITermux 的终端 AI 工作台，面向 Termux/Android 环境开发。

它不是通用桌面程序，也不建议普通用户直接尝试。

它用于实验性，AI前沿技术爆破

上下文工程设计与Agent协同

基于第三方Codex API，暂未适配任何其它API。

也就是说，只支持中转站的Codex。

功能：

Matrix母体Agent调度

多Agent协同

永久记忆与Matrix体系

服务器运维

编程

母体分裂技术

专注模式交叉上下文

动态上下文

上下文治理工程

三层永久记忆机制

Agent自优化系统

AIdebug智能系统

matrix母体分裂系统

子Agent调度系统

matrix自生长系统

TERMUX终端触控

对账策略系统与升级蓝图计划工具

fastmemory表层记忆系统

多层压缩机制

... 

等


## 入门门槛要求

- Android + Termux
- 已安装 AITermux
- 基础 Linux/Termux 使用能力
- 能理解 API Key、模型代理、文件权限和终端日志
- 部分手机自动化、ADB、服务器管理能力可能需要额外授权、无线调试或 root 环境
- 计算机理论基础
- AI知识与Agent知识
- 开发者基础知识


## 启动

通常由 AITermux 启动器拉起：

```bash
cd ~/AItermux/projectying
./run.sh
```

首次启动会在本地生成运行配置、上下文、记忆和日志。不要把这些运行态文件提交到仓库。

## 本地构建

```bash
pkg install rust clang make pkg-config
cargo build --release
```

## 仓库边界

- 只支持 Termux/AITermux 链路。
- 无法在 Linux 桌面、Windows、macOS 或普通 Android shell 中运行。
- 使用前先阅读源码和配置，确认你知道它会调用哪些工具。
