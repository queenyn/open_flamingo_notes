# 🧠 OpenFlamingo-Learning

本项目是我个人对 [OpenFlamingo 多模态大模型](https://github.com/mlfoundations/open_flamingo) 的系统性学习与结构研究过程，目标是掌握现代多模态系统的核心组件，实现模块替换与实验对比，并在未来实习阶段具备撰写论文的能力。

---
---

## 📚 学习路线

以下五个模块构成了我当前阶段的学习路线，每个模块包含多个知识点与实际实验。

| 模块 | 说明 |
|------|------|
| [图像编码器](./experiment_logs/01_vision_encoder/) | ViT、ResNet、CLIP，理解输入处理、结构与替换方案 |
| [文本编码器](./experiment_logs/02_text_encoder/) | Transformer/LLaMA 结构与注意力机制，处理 prompt |
| [自监督与对比学习](./experiment_logs/03_ssl_contrastive/) | SimCLR / MAE / BYOL 等训练目标与视觉预训练思想 |
| [多模态融合机制](./experiment_logs/04_multimodal_fusion/) | Cross-Attention、Perceiver Resampler、Prompt 拼接 |
| [实验管理与调试](./experiment_logs/05_experiment_management/) | PyTorch 训练流程、wandb、模型替换控制实验设计 |

---

## ✅ 当前进度

📌 项目正在进行中，学习进度见 [tasks_todo.md](./tasks_todo.md)

---

## 📁 仓库结构说明

- `flamingo/`：fork 的原始多模态模型代码
- `exploration/`：每个模块的学习笔记与实验记录
- `notebooks/`：结构调试与可视化 notebook
- `results/`：输出样例与可视化图表
- `README.md`：学习路径与项目简介

---

## 📌 示例展示（部分）

| 实验 | 内容 | 状态 |
|------|------|------|
| 替换视觉编码器为 CLIP-L/14 | 观察 token shape 变化、输出稳定性 | ✅ 完成 |
| 打印文本 token 到嵌入矩阵流程 | 理解 tokenizer + embedding | ✅ 完成 |
| 复现 MAE 遮挡重建过程 | 将 MAE 表示替换进 OpenFlamingo | ⏳ 进行中 |

---
> 本项目 Fork 自 [OpenFlamingo](https://github.com/mlfoundations/open_flamingo)
