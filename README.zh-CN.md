# DCL (Data Commons Language)

**版本 1.0.0 · 正式发布**

一个开放、中立、可扩展的 AI 数据访问协议。  
完全兼容 [Model Context Protocol (MCP)](https://github.com/anthropic/mcp)。

---

## 概述

DCL 定义了大语言模型（客户端）与数据源（服务器）之间的通用通信语法——包括文件系统、数据库、云存储、应用程序接口。

它基于三个核心设计原则：

- **兼容优先** —— DCL 1.0 是 MCP 的超集。每个 DCL 实现都完全支持标准 MCP。
- **可选设计** —— 所有 DCL 扩展字段均为可选，不会破坏现有 MCP 生态。
- **默认透明** —— DCL 要求对排序逻辑和权限摘要提供人类可读的解释。

---

## 协议栈

| 层级 | 名称 | 状态 | 描述 |
|------|------|------|------|
| L1 | 传输语法 | **1.0.0 稳定版** | 请求/响应格式、鉴权、元数据 |
| L2 | 身份语法 | 草案阶段 | 分布式身份标识与跨域迁移 |
| L3 | 许可语法 | 规划阶段 | 数据使用条件声明 |

---

## 快速开始

### 1. 阅读规范
完整协议规范：[`PROTOCOL.zh-CN.md`](./PROTOCOL.zh-CN.md)

### 2. 参考实现
- Python（开发中）
- TypeScript（开发中）

### 3. 社区与贡献
- Issues 与讨论：GitHub Issues
- 贡献指南：[`CONTRIBUTING.zh-CN.md`](./CONTRIBUTING.zh-CN.md)

---

## 仓库

| 角色 | 平台 | 地址 |
|------|------|------|
| **主仓库** | GitHub | https://github.com/zhiencloub/dcl |
| 镜像（中国） | Gitee | https://gitee.com/dcl-org/dcl |

---

## 许可证

- **代码**：MIT 许可证
- **文档**：CC BY 4.0
- **协议规范**：公共领域

---

## 维护者

DCL 由开源社区维护。初始提案由中国开发者贡献，欢迎全球贡献者与采用者。
