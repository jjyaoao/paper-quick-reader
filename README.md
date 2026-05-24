# paper-quick-reader

论文快速阅读助手 RedSkill。

它用于快速阅读和结构化理解学术论文。用户提供论文标题、摘要、PDF 文本、arXiv 链接、截图、方法段落或相关代码仓库时，Skill 会输出一份面向学习者和研究者的快速阅读笔记。

## 适合场景

- 判断一篇论文值不值得深读
- 准备组会或课程汇报
- 写 related work 或开题文献综述
- 论文复现前快速理解方法和实验
- 快速整理论文的核心问题、方法、局限和下一步阅读路线

## 输出内容

- 一句话结论
- 论文基本信息
- 论文想解决的问题
- 核心想法
- 方法结构拆解
- 实验到底证明了什么
- 局限和风险
- 是否值得深读
- 下一步阅读建议
- 组会讲法
- Related Work 写法

## 文件结构

```text
.
├── SKILL.md
├── demo-react.md
└── references/
    ├── note-template.md
    ├── paper-types.md
    └── reading-modes.md
```

## 使用示例

```text
请使用“论文快速阅读助手”这个 Skill，帮我快速阅读 ReAct 这篇论文。

论文：ReAct: Synergizing Reasoning and Acting in Language Models
论文链接：https://arxiv.org/abs/2210.03629
官方代码：https://github.com/ysymyth/ReAct

我的目标：
1. 先判断这篇论文值不值得深读。
2. 我关注 Agent、Tool Use 和论文复现。
3. 输出包括：一句话结论、核心想法、方法结构、实验证明了什么、局限、是否值得读、下一步阅读建议。
```

完整演示见 [demo-react.md](demo-react.md)。

## License

MIT
