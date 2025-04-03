# YYH Chat 项目

这是一个基于 C++ 开发的分布式聊天系统项目，涵盖了 gRPC、并发线程、网络编程、Qt 开发、数据库等多种技术的综合应用。

## 项目结构

```
.
├── client/                 # 客户端代码
│   └── yyhchat/          # Qt 实现的聊天客户端
├── server/                 # 服务端代码
│   ├── ChatServer/        # 聊天服务器
│   ├── ChatServer2/       # 聊天服务器2
│   ├── GateServer/        # 网关服务器
│   ├── StatusServer/      # 状态服务器
│   └── VarifyServer/      # 验证服务器
└── sql备份/               # 数据库备份文件
```

## 系统架构

本项目采用分布式架构设计，主要包含以下组件：

1. **客户端 (Client)**

   - 基于 Qt 框架开发
   - 提供用户界面和交互功能
   - 负责与服务器通信
   - 支持 TCP 和 HTTP 协议

2. **服务端 (Server)**
   - ChatServer/ChatServer2: 处理聊天消息的核心服务
   - GateServer: 负责请求转发和负载均衡
   - StatusServer: 管理用户状态和在线信息
   - VarifyServer: 处理用户认证和授权

## 技术栈

- **客户端**

  - Qt 框架
  - C++ 11/14
  - HTTP 客户端
  - TCP 客户端

- **服务端**

  - gRPC 框架
  - Boost.Asio 网络库
  - Beast HTTP 服务器
  - Redis 缓存
  - MySQL 数据库

- **开发工具**
  - Visual Studio
  - CMake
  - Git

## 主要功能

- 用户注册和登录
- 邮箱验证
- 好友管理
- 实时聊天
- 消息历史记录
- 在线状态管理

## 开发环境要求

- 操作系统：Windows 10/11
- 开发工具：Visual Studio 2019+
- 依赖库：
  - Boost
  - gRPC
  - Qt
  - Redis
  - MySQL

## 安装和运行

1. 克隆项目

```bash
git clone [项目地址]
```

2. 安装依赖

- 安装 Visual Studio
- 安装 Qt
- 安装 Boost
- 安装 gRPC
- 安装 Redis
- 安装 MySQL

3. 编译项目

```bash
mkdir build
cd build
cmake ..
make
```

4. 运行服务

- 启动 Redis
- 启动 MySQL
- 启动各个服务器组件
- 运行客户端程序

## 项目特点

- 分布式架构设计
- 多服务器协同工作
- 可扩展性强
- 高可用性设计
- 支持高并发
- 实时消息推送

## 贡献指南

欢迎提交 Issue 和 Pull Request 来帮助改进项目。

## 许可证
