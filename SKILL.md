---
name: xxxx
title: xxxx
description: xxxx —— 由 CruiseSkillBridge 一键发布的MCP。
kind: MCP
version: 0.1.0
published_with: cruiseskillbridge
---

# xxxx

> xxxx —— 由 CruiseSkillBridge 一键发布的MCP。

这是一个 **MCP** 技能，通过 [CruiseSkillBridge](https://cruiseskillbridge.com) 一键发布。

## 能力

- 描述这个技能能做什么（请替换为你的真实内容）。
- 列出关键输入与输出。
- 说明适用场景。

## 用法

当需要提交分析请求时，向以下 API 发送 **POST** 请求（JSON body）：

```
https://httpbin.org/post
```

示例 body：

```json
{ "input": "...", "skill": "xxxx" }
```

> 发布到 CruiseSkillBridge 后，上述 URL 会自动替换为网关地址，调用将计入控制台统计。

## 关于

由 [CruiseSkillBridge](https://cruiseskillbridge.com) 发布 —— 全球唯一邮轮领域技能 分发 · 发布 · 洞察：
一键发布、分发洞察、网关调用统计。

## 已发布的 MCP Tools

以下 Tools 已纳入 CruiseSkillBridge 发布与统计：

- **freellm_get_video_status** — 
    查询 FreeLLM 视频任务状态（配合 freellm_create_video_task 使用）。

    Args:
        task_id: 创建任务返回的 task_id
        video_id: 可选，创建任务返回的 video_id
    
- **freellm_create_video_task** — 
    仅创建文生视频任务（不等待完成）。返回 task_id / video_id，可用 freellm_get_video_status 轮询。

    Args:
        prompt: 视频描述
    

> MCP 接入经 CruiseSkillBridge 网关转发，remotes URL 已自动替换，无需手动配置。
