---
layout: post
title: AI学习笔记（一） 学习路线图
date: 2025-02-01 22:52 +0800
description:
image:
category: AI学习笔记
tags:
---
### 核心理念

- **实践驱动**: 理论结合编码实践，多做项目。
- **循序渐进**: 从基础到进阶，逐步构建知识体系。
- **善用背景**: 发挥你的软件工程和 Azure 优势。
- **拥抱英文**: AI 领域优质资源以英文为主。
- **持续学习**: 技术日新月异，保持好奇心。

---

### AI 工程师学习路线图 (整合版)

#### 阶段 0: 基础巩固 (查漏补缺)

**目标**: 确保 Python 和数学基础扎实。

**内容**:
- **Python 进阶**: 面向对象编程、装饰器、生成器、异步编程 (如果需要)、常用标准库。
  - **资源**: 《Fluent Python》, Python 官方文档, LeetCode/HackerRank 练习。
- **核心数学**: 线性代数、微积分、概率与统计 (达到理解算法原理的程度即可)。
  - **资源**: Khan Academy, 3Blue1Brown (YouTube), MIT OpenCourseware, 《统计学习方法》附录。

---

#### 阶段 1: 核心机器学习基础

**目标**: 掌握经典机器学习算法、数据处理和模型评估。

**内容**:
- **NumPy & Pandas**: 精通数据操作、清洗、分析。
  - **资源**: 官方文档, Kaggle Learn (NumPy, Pandas), 《Python for Data Analysis》。
- **Scikit-learn**: 掌握常用算法 (线性/逻辑回归, SVM, 树模型, 聚类), 数据预处理, 特征工程, 模型选择 (交叉验证), 评估指标。
  - **资源**: Scikit-learn 官方文档 (非常棒!), 《Hands-On Machine Learning》(Geron) 第一部分, 吴恩达《机器学习》课程 (理解概念)。
- **数据可视化**: Matplotlib, Seaborn 用于理解数据和结果。
  - **资源**: 官方文档, Kaggle Learn (Data Visualization)。

---

#### 阶段 2: 深度学习基础

**目标**: 理解神经网络原理，掌握至少一个主流深度学习框架。

**内容**:
- **神经网络基础**: 感知机、反向传播、激活函数、损失函数、优化器 (SGD, Adam)。
- **深度学习概念**: 过拟合/欠拟合、正则化、Dropout、批量归一化 (Batch Norm)。
- **深度学习框架** (精通其一，了解另一个):
  - **TensorFlow (Keras)**: 适合生产部署。
  - **PyTorch**: 研究领域更流行，灵活。
  - **资源**: 吴恩达《深度学习》专项课程 (理论), 《Hands-On Machine Learning》(Geron) 第二部分 (实践, TF/Keras), PyTorch/TensorFlow 官方教程。

---

#### 阶段 3: 自然语言处理 (NLP) 与 Transformer/LLM 专项

**目标**: 掌握 NLP 核心技术，深入理解 Transformer，能够使用和微调大语言模型。

**内容**:
- **NLP 基础回顾**: 词嵌入 (Word2Vec/GloVe), RNN/LSTM/GRU 原理。
  - **资源**: Stanford CS224n (可选深入), 相关博客图解。
- **Transformer 核心**:
  - **理论**: 精读 "Attention Is All You Need" 论文，理解 Self-Attention, Multi-Head Attention, Positional Encoding, Encoder/Decoder 结构。
  - **资源**: Jay Alammar 图解博客 ("Illustrated Transformer"等), Harvard "Annotated Transformer"。
- **Hugging Face 生态系统**:
  - **transformers 库**: 加载、使用、微调各种预训练模型 (BERT, GPT, T5, Llama, DeepSeek 等)。
  - **datasets 库**: 加载和处理数据。
  - **Hugging Face Hub**: 模型和数据集中心。
  - **资源**: Hugging Face Course (必学!), 官方文档。
- **大语言模型 (LLM) 概念与应用**:
  - **关键模型架构**: 理解 BERT, GPT 系列, T5, Llama 等。
  - **应用技术**:
    - 微调 (Fine-tuning): 使用 transformers 库进行下游任务适配。
    - 提示工程 (Prompt Engineering): 设计有效提示。
    - 检索增强生成 (RAG): 结合外部知识 (学习 LangChain/LlamaIndex 基础)。
    - 参数高效微调 (PEFT): LoRA, QLoRA 等 (学习 peft 库)。
  - **资源**: Hugging Face Course, 相关论文, LangChain/LlamaIndex 文档, peft 文档。

---

#### 阶段 4: MLOps 与生产化 (工程核心)

**目标**: 掌握将模型部署到生产环境并维护的技术。

**内容**:
- **SQL**: 熟练数据提取。
  - **资源**: Mode Analytics SQL Tutorial, LeetCode/SQLZoo 练习。
- **容器化**: Docker (打包模型和依赖)。
  - **资源**: Docker 官方 Get Started。
- **编排**: Kubernetes (部署和管理容器)。
  - **资源**: Kubernetes Basics 官方教程, CKAD/CKA 备考资源。
- **云平台 (重点 Azure)**:
  - **Azure Machine Learning (AML)**: 工作区、数据集、计算、管道、模型注册、端点部署 (在线/批量)。
  - **相关服务**: Azure Kubernetes Service (AKS), Azure Databricks (大规模数据处理/训练), Azure Functions (Serverless), Azure Blob/Data Lake Storage。
  - **资源**: Microsoft Learn (Azure AI Engineer/Data Scientist/ML 学习路径), Azure 官方文档。
  - **CI/CD**: GitHub Actions, Azure DevOps Pipelines (自动化构建、测试、部署流程)。
  - **资源**: 各工具官方文档, 搜索 "CI/CD for ML"。
  - **实验跟踪与版本控制**: MLflow (推荐), DVC, Weights & Biases。
  - **资源**: 各工具官方文档。
  - **模型服务**: TensorFlow Serving, TorchServe, FastAPI/Flask (构建 API), 云平台端点, (了解 vLLM, TGI 等 LLM 高性能推理框架)。
  - **资源**: 各工具/框架文档。
  - **监控**: Prometheus, Grafana, 云平台监控工具 (监控模型性能、漂移、资源)。
  - **资源**: 各工具官方文档, MLOps 课程。
  - **综合 MLOps 学习资源**: MLOps Zoomcamp, Full Stack Deep Learning。

---

#### 阶段 5: 软件工程实践与系统设计

**目标**: 将软件工程的最佳实践应用到 AI 项目中，具备设计复杂系统的能力。

**内容**:
- **Git**: 精通版本控制。
  - **资源**: 《Pro Git》, Learn Git Branching。
- **测试**: 单元测试 (pytest), 集成测试, 数据验证, 模型评估的稳健性测试。
  - **资源**: pytest 文档, 《Test-Driven Development with Python》。
- **API 设计**: 设计健壮的 RESTful API。
  - **资源**: Google/Microsoft API 设计指南, FastAPI/Flask 教程。
- **代码质量**: Clean Code 原则, PEP 8, 类型提示 (Type Hinting)。
  - **资源**: 《Clean Code》, Flake8/Black 工具。
- **系统设计**:
  - **通用系统设计**: 可扩展性、可靠性、性能权衡。
  - **ML 系统设计**: 端到端流程设计 (数据管道、训练、部署、监控), 在线/离线系统, 特征存储, A/B 测试。
  - **资源**: 《Designing Data-Intensive Applications》, System Design Primer, Grokking the System Design Interview, 搜索 "ML System Design Interview"。

---

### 贯穿始终 (Ongoing)

**项目实践**:
- **个人项目**: 将所学应用于解决实际问题（Kaggle 数据集或自选题目），构建端到端的项目并放到 GitHub。
- **Kaggle 竞赛**: 参与 NLP 或其他相关竞赛，学习他人代码。
- **论文阅读**: 关注顶会 (ACL, EMNLP, NeurIPS, ICML 等) 和 arXiv 上的最新进展。
- **社区参与**: 加入技术社区，阅读博客，关注行业专家。
- **网络构建**: 与同行交流