---
name: character-lock
title: 角色定妆锁定
agent: makeup
version: 0.1.0
lang: zh-CN
max_chars: 4500
---

# 角色定妆锁定（Character Sheet）

## 何时使用

- 有参考图或已锁定人设，需要一张**高精度角色设定板**，供后续分镜出图 / 图生视频锁同一角色 ID。
- 禁止在无参考、无文字人设时凭空新造脸。

## 目标输出

一张 **4:3 横版**、背景纯白/米白/极简的设定板。干净技术排版：无 logo、无水印。标签用清晰可读英文。
主身份展示区必须是画面最大区域。

## 输入（填齐再画）

- 参考图（必填；多角度更好）或已锁定文字人设
- 风格：写实3D / 风格化3D / 动漫 / 半写实 / IP设计（择一）
- 性别、年龄、体型
- 风格关键词（如高级感、时尚、科技感、情绪化）
- 可选：名字、身份、性格关键词；缺则按参考合理补全并写进顶部信息

## 步骤

1. 从参考抽稳定特征：脸型、五官、发型发色、肤色、体型比例、服装与材质。写成内部「角色锁」短描述，后续模块只复用，不改写。
2. 定画幅与排版：4:3 横版；主展示区最大；其余模块围绕主区，不抢戏。
3. 按下方模块一次出齐；同一张图内角色完全一致（脸/发型/比例/服装），禁止风格漂移、禁止生成新角色。
4. 自检：任意子图裁出来仍能认成同一人；主区有比例线；无道具干扰主身份展示。

## 必须包含模块

1. **顶部信息**：名字、身份、年龄、性格关键词 3–5 个、核心主题 1 句
2. **配色系统**：6–8 个色块，无文字
3. **主身份展示（最大）**：正面 / 3/4 / 侧面 / 背面；标准站姿；带身高比例线；无道具
4. **轮廓剪影**：正面、侧面
5. **表情系统（8）**：平静、好奇、紧张、惊讶、害怕、悲伤、坚定、放松
6. **微表情（5）**：眼部紧张、微笑、嘴部用力、微恐惧、呼吸控制
7. **头部结构**：多角度（3/4、侧面、仰视、俯视）
8. **姿态变化**：放松、紧张、自信
9. **特写（1）**：胸部以上，强情绪
10. **服装细节（4）**：发型、材质、配饰、鞋
11. **手部动作**：放松、紧张、指向、抓握、面部相关手势

## 硬约束 / 禁止

- 所有子画面必须基于同一角色结构；不允许生成新角色或换脸换发型换装。
- 不允许风格漂移（写实突然变二次元等）。
- 主展示区必须最大；不要被表情墙或细节格压过。
- 无 logo、无水印、无中文乱码标签（标签用英文）。
- 材质真实（皮肤/布料/金属），影视级光影；细节要足，但禁止用「0G级」等夸张空话当指令。

## 出图提示写法（给下游）

先锁角色短描述，再写 layout 与模块列表；英文标签名固定。示例骨架（按输入替换括号内容）：

```text
Character sheet, 4:3 landscape, clean technical layout on off-white background, no logo no watermark.
LOCKED CHARACTER: (face/hair/body/outfit from reference — do not invent a new person)
Style: (chosen style). Gender (x), age (n), build (x). Keywords: (...)
Header: name, role, age, 3-5 personality tags, one-line theme.
Color system: 6-8 swatches, no text.
Largest zone — turnaround: front, 3/4, side, back; T-pose/standard stance; height proportion lines; no props.
Silhouettes: front + side.
Expression grid (8): calm, curious, tense, surprised, scared, sad, determined, relaxed.
Micro-expressions (5): eye tension, smile, mouth strain, slight fear, breath control.
Head studies: 3/4, profile, low angle, high angle.
Poses: relaxed, tense, confident.
One emotional bust close-up.
Costume details (4): hair, fabric, accessories, shoes.
Hands: relaxed, tense, pointing, gripping, face-touch.
Same identity everywhere; cinematic lighting; realistic materials.
```

## 质检清单

- [ ] 有参考或已锁定人设，未凭空新造脸
- [ ] 4:3 横版，背景极简，无 logo/水印
- [ ] 主身份展示区最大，含正/3-4/侧/背 + 比例线、无道具
- [ ] 11 类模块齐全；表情 8 + 微表情 5
- [ ] 全图同一角色、同一服装、同一风格
- [ ] 英文标签清晰可读
