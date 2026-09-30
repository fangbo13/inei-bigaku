# 陰翳美学（inei-bigaku / Shadowism）

> 「美は物体にあるのではなく、物体と物体との作り出す陰翳のあや、明暗にある」——谷崎潤一郎『陰翳礼讃』

基于谷崎润一郎《阴翳礼赞》东方幽玄哲学的 AI 画风转换与艺术再诠释 Skill。

---

## 目录结构

```text
├── inei-bigaku/
│   ├── SKILL.md                          # 技能主指令与核心规范
│   ├── evals/
│   │   └── evals.json                    # 测试用例与评估基准
│   └── references/
│       ├── aesthetics.md                 # 《阴翳礼赞》美学原理与题材对照表
│       ├── masters.md                    # 视觉大师参照（王家卫、宫川一夫、霍珀等）
│       ├── optics-and-palette.md         # 文学到光学渲染语言对照表与色彩规范
│       └── prompt-templates.md           # Gemini / Midjourney / SD 专属提示词模板
├── inei-bigaku.skill                     # 打包分发文件
└── README.md
```

## 核心设计原则

1. **构图大减法（Subtractive Composition）**：斩断杂物与商品陈列感，画面 75% 浸入富有呼吸感的层叠暗影。
2. **光之刺点（Punctum）**：暗夜中必有一处摄人心魄的微光（熏金莳绘、若隐若现的水汽、或玉石白瓷的内蕴透光）。
3. **光学工程化（Optics Translation）**：将文学修辞转化为扩散模型可精确理解的物理光学语言（次表面散射 `subsurface scattering`、微划痕哑光包浆 `micro-scratched matte patina`、平方反比光线衰减 `inverse-square falloff` 等）。
4. **两重境界**：
   - **【残光·清寂】**：冷色天窗/障子透光、极简素陶、袅袅茶汽。
   - **【金幽·绚烂】**：低位烛火、黑漆浓夜、熏金莳绘微芒。

## 适用平台
- Google Antigravity / Gemini
- Midjourney
- Stable Diffusion / Flux
