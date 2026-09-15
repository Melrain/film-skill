# Skill 文件约定

每个 Skill 一个目录：`skills/<id>/SKILL.md`。

## Frontmatter

```yaml
---
name: video-parse
title: 爆款视频解析
agent: parse
version: 0.1.0
lang: zh-CN
max_chars: 4000
---
```

## 正文建议章节

1. 何时使用
2. 目标输出
3. 步骤
4. 硬约束 / 禁止
5. 输出格式
6. 质检清单

## 写作原则

- 面向 R7 现有产物（镜号卡、文字资产描述、卡内出图），勿写假指标或营销话术。
- 正文宜短；细则可日后放 `references/` 按需加载。
- 开源 Skill 只作结构参考，禁止大段照搬。
