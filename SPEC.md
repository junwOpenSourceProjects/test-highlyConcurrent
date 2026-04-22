# SPEC.md - test-highlyConcurrent

## 1. 项目概述

- **项目名称**: test-highlyConcurrent
- **项目类型**: Spring Boot WebFlux 项目
- **核心功能**: 高并发场景测试项目，使用 WebFlux + Netty 实现异步非阻塞响应式编程
- **目标用户**: 需要测试高并发性能的开发者

## 2. 技术栈

| 组件 | 版本 |
|------|------|
| Spring Boot | 3.3.0 |
| Java | 17 |
| Spring WebFlux | 3.3.0 ( Netty 嵌入式服务器) |

## 3. 功能规格

### 3.1 核心功能

- **异步非阻塞**: 使用 Spring WebFlux 实现响应式编程
- **Netty 服务器**: 使用 Netty 作为嵌入式服务器替代 Tomcat
- **高并发处理**: 支持高并发场景下的异步请求处理

### 3.2 项目结构

```
src/main/java/wo1261931780/st_highlyConcurrent/
└── StHighlyConcurrentApplication.java    # Spring Boot 启动类
```

### 3.3 依赖说明

| 依赖 | 说明 |
|------|------|
| spring-boot-starter-webflux | 提供响应式 Web 框架，使用 Netty |
| spring-boot-starter-web (已排除 Tomcat) | 排除默认 Tomcat，使用其他容器 |

### 3.4 配置

- **Java 版本**: 17
- **编码格式**: UTF-8
- **端口**: 默认 8080

## 4. 编译信息

- **Maven 编译**: 通过
- **打包方式**: JAR

## 5. README.md 状态

- 存在，包含架构图、并发测试流程图、性能优化策略图
- 内容较为完整，是一份技术演示文档

## 6. .gitignore 状态

- 存在但不够完整，缺少内容同 demo-analysisJsonToObject
