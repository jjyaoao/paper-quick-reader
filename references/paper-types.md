# 常见论文类型阅读关注点

## LLM Agent / Tool Use

关注：

- agent 循环如何定义
- action space 有哪些
- observation 如何进入上下文
- 工具调用是否稳定
- 评价指标是否只看最终答案

常见风险：

- 只展示成功轨迹
- 搜索结果不稳定
- prompt 过拟合示例
- baseline 不公平

## LLM Fine-tuning / Adapter

关注：

- 冻结哪些参数
- 训练哪些参数
- 数据量和训练预算
- 参数效率和效果如何权衡
- 和 full fine-tuning 是否公平比较

常见风险：

- seed 波动
- 只报单次结果
- 训练预算不一致
- 忽略显存和时间成本

## RAG / Retrieval

关注：

- 检索器是什么
- 文档库如何构建
- rerank 是否使用
- 生成模型如何接收 evidence
- hallucination 如何评估

常见风险：

- 检索失败和生成失败混在一起
- 文档库版本不固定
- citation correctness 不检查

## Computer Vision

关注：

- 数据增强
- backbone
- loss
- 推理成本
- 训练 recipe
- 和同规模模型是否公平比较

常见风险：

- 改动来自训练技巧而不是方法本身
- 没有报告计算成本
- 数据预处理细节缺失

## Recommendation / Ranking

关注：

- 数据切分方式
- negative sampling
- ranking metric
- cold-start 或 long-tail 表现
- online/offline gap

常见风险：

- 数据泄漏
- 采样方式不一致
- 只看总体指标

## Time Series

关注：

- 输入窗口
- 预测 horizon
- 数据标准化
- rolling split
- naive baseline

常见风险：

- 切分方式导致泄漏
- horizon 不可比
- 缺少简单 baseline

