---
layout: post
title: AI学习笔记（一） 
date: 2025-02-01 22:52 +0800
description:
image:
category: AI学习笔记
tags:
---

### **一、基础准备**
1. **数学基础**
   - **线性代数**：矩阵运算、特征值、张量等（大模型的核心是矩阵计算）。
   - **概率与统计**：概率分布、贝叶斯定理、极大似然估计等。
   - **微积分**：梯度、导数、优化方法（如梯度下降）。
   - **信息论**（可选）：交叉熵、KL散度等（用于理解模型损失函数）。

2. **编程能力**
   - **Python**：AI领域的主流语言，需熟悉NumPy、Pandas等库。
   - **深度学习框架**：PyTorch（大模型开发首选）或TensorFlow。
   - **并行计算基础**：了解GPU加速（CUDA）和多进程编程。

3. **机器学习基础**
   - **经典算法**：线性回归、决策树、SVM、聚类等。
   - **深度学习基础**：神经网络、反向传播、CNN（图像）、RNN/LSTM（序列数据）。
   - **优化方法**：随机梯度下降（SGD）、Adam、学习率调整等。

---

### **二、深度学习进阶**
1. **核心架构**
   - **Transformer**：大模型的基石，需掌握Self-Attention、位置编码、多头注意力机制。
   - **BERT/GPT**：理解预训练（Pretraining）和微调（Finetuning）范式。
   - **扩散模型**（Diffusion Models）：图像生成领域的核心模型（如Stable Diffusion）。
   - **多模态模型**（如CLIP、DALL-E）：文本与图像的联合建模。

2. **关键技术**
   - **预训练技术**：Masked Language Modeling（MLM）、Next Sentence Prediction（NSP）。
   - **模型蒸馏**（Distillation）：将大模型压缩为小模型。
   - **高效训练技术**：混合精度训练、梯度检查点（Gradient Checkpointing）、分布式训练（如ZeRO、DeepSpeed）。
   - **提示工程**（Prompt Engineering）：设计有效提示词以引导模型输出。

---

### **三、大模型专项学习**
1. **经典论文与模型**
   - **必读论文**：
     - 《Attention Is All You Need》（Transformer原论文）。
     - 《BERT: Pre-training of Deep Bidirectional Transformers》。
     - 《Language Models are Few-Shot Learners》（GPT-3）。
     - 《Training Compute-Optimal Large Language Models》（Chinchilla）。
   - **主流模型**：GPT系列、LLaMA、PaLM、T5、Stable Diffusion等。

2. **训练与部署**
   - **数据工程**：清洗、去重、构建高质量预训练数据集。
   - **分布式训练**：数据并行、模型并行、流水线并行。
   - **模型压缩**：量化（Quantization）、剪枝（Pruning）。
   - **推理优化**：使用ONNX、TensorRT加速推理。

3. **工具与框架**
   - **Hugging Face**：Transformers库、Datasets库、模型Hub。
   - **分布式训练框架**：DeepSpeed、Megatron-LM。
   - **云平台**：AWS/GCP/Azure的GPU实例，或Colab/Kaggle免费资源。

---

### **四、实践项目**
1. **从小项目开始**
   - 用Hugging Face微调BERT/GPT-2完成文本分类、生成任务。
   - 复现经典论文的简化版（如手写Transformer）。
   - 使用LangChain构建基于大模型的AI应用（如聊天机器人）。

2. **进阶挑战**
   - 参与Kaggle竞赛（如NLP或生成类比赛）。
   - 训练小型大模型（如从头训练一个百亿参数的模型）。
   - 部署模型到生产环境（如使用FastAPI+ Docker）。

3. **开源贡献**
   - 参与大模型相关开源项目（如LLaMA、Alpaca、Stable Diffusion）。
   - 在GitHub上分享自己的代码和模型。

---

### **五、持续学习与社区**
1. **跟踪前沿**
   - 关注顶会论文：NeurIPS、ICML、ICLR、ACL、CVPR。
   - 订阅arXiv每日更新，关注`cs.CL`（自然语言处理）、`cs.LG`（机器学习）板块。
   - 关注AI实验室动态：OpenAI、DeepMind、Meta AI、Google Brain。

2. **学习资源**
   - **课程**：
     - 吴恩达《Deep Learning Specialization》（Coursera）。
     - 李沐《动手学深度学习》（中文，B站/书）。
     - Hugging Face官方课程（免费）。
   - **书籍**：
     - 《Deep Learning》（花书）。
     - 《Natural Language Processing with Transformers》。

3. **社区与交流**
   - 加入AI社群（如知乎、Reddit的r/MachineLearning、Hugging Face论坛）。
   - 参与AI Meetup或学术会议（线上/线下）。