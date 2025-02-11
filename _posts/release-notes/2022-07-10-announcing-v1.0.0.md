---
layout: post
title: Announcing Hango 1.0.0
subtitle: Hango v1.0.0 release announcement.
cover-img: /assets/img/cover/natual-scene-1.png
thumbnail-img: /assets/img/hango/gateway.jpeg
share-img: /assets/img/hango/gateway.jpeg
tags: [release-notes]
---

本次更新是Hango正式版V1.0的发布。在去年11月发布的基础上进行了架构升级，适配了Istio1.12+的版本，推出EnvoyPlugin以及PluginManagers两个新的Slime CRD，从功能以及扩展度上都进行了整体的升级。

### 新功能

- 支持服务维度的负载均衡配置，包括轮询、最小连接、一致性Hash

- 支持版本分流

- 支持服务维度主动/被动健康检查

- 支持TCP/HTTP连接池配置

- 支持空闲超时

- 支持路由维度重试

- 支持动态降级、静态降级配置

- 支持根据错误码以及慢响应的熔断配置

- 支持本地限流

- 支持多维度黑白名单配置,包括UA黑白名单，IP黑白名单，Refer黑白名单以及自定义Header黑白名单

- 支持服务/路由维度指标监控

- 对接skywalking、prometheus的链路追踪及指标能力


### 工程增强

- 一键helm部署及初始化，脱离istioctl，直接采用helm部署，部署完成后，自动进行初始化

- 采用Istio1.12+版本，升级Rider模块，支持异步获取请求body

- 优化rider lua FFI，lua扩展性能进一步提升

