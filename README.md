# R7 Film Skills

R7 影片工作台的**官方方法库种子**：给画布智能体（视频解析、续写剧本、分镜出图等）挂接的可复用 Skill 正文。

- 格式见 [FORMAT.md](./FORMAT.md)
- 开源参考来源见 [SOURCES.md](./SOURCES.md)（只借结构，正文为 R7 原创）
- Skill 索引见 [skills/README.md](./skills/README.md)

## 和产品的关系

| 概念 | 说明 |
|------|------|
| Skill | 一份 `SKILL.md`：步骤、约束、输出格式 |
| 画布连线 | 日后 Skill 节点可连到智能体；未接时用目录默认短 prompt |
| 注入 | Nest 侧把 Skill 正文拼进该次任务指令（需产品接线后生效） |

当前仓库是**内容种子**，不含 Nest/Next 接线代码。

## P0（已收录）

1. `video-parse` — 爆款视频解析
2. `script-continue` — 跟拍续写剧本
3. `shot-image` — 分镜卡出图
4. `character-lock` — 角色定妆锁定

## 规划中（P1）

镜头语言导演、短视频节奏 — 见 skills 索引，正文后补。

## License

MIT
