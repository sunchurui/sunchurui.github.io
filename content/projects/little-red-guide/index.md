---
title: 小红导览机器人：基于多模态知识库的智能问答系统
summary: 面向实时游客问答场景，基于混合检索架构与Qwen-Reranker的多模态智能导览系统。
tags:
  - RAG
  - 多模态
  - 智能问答
date: '2024-04-01'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: video
    icon_pack: fas
    name: 演示视频
    url: '#'
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

**时间**: 2024.04 -- 2024.06

### 项目背景
面向哈工大中心实时游客问答场景，传统关键词检索难以应对复杂、口语化的用户提问，且缺乏对上下文的理解。本项目旨在构建一个高精度、快速响应的智能问答导览机器人。

### 核心工作
*   **混合检索架构**: 
    *   在非 GPU 环境下，自主研发基于分词与关键词匹配的规则引擎，保障基础响应能力。
    *   在 GPU 环境下，采用 **BGE** 向量模型进行深层语义检索，并引入 **Qwen-Reranker** 对召回结果进行重排序，大幅提升检索准确率。
*   **上下文感知优化**: 集成对话历史感知的问题重写机制，并结合父子文档索引策略，有效解决了多轮对话中指代不明和上下文依赖的问题。
*   **系统落地与成效**: 系统成功上线哈工大中心，单日最高服务游客数达 **1.2 万人次**。配套宣传视频在社交媒体获得 1000+ 点赞与 890+ 转发，展现了良好的社会影响力。

