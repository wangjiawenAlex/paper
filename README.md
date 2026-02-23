# 混合检索与动态路由相关文献

- **标题**：Retrieval-Augmented Generation with Knowledge Graphs for Customer Service Question Answering
  **作者**：Zhentao Xu, Mark Jerome Cruz, Matthew Guevara, Tie Wang, Manasi Deshpande, Xiaofeng Wang, Zheng Li
  **年份**：2024
  **出处**：SIGIR 2024 (International ACM SIGIR Conference on Research and Development in IR)
  **链接**：arXiv:2404.17723 (预印本)
  **推荐理由**：该文提出了一种将 RAG 与知识图谱相结合的问答方法，将历史客服故障工单构建为知识图谱并用于检索，通过解析用户查询并检索相关子图生成答案，从而保留了工单内部结构与工单间关系。实验表明此方法显著提升检索准确率与答案质量（MRR 提升 77.6%、BLEU 提升 0.32），在实际客服场景中亦验证了效果。该研究直接结合向量检索（文本）与图谱检索技术，符合“知识图谱与语义检索融合”主题。
- **标题**：SG-RAG: Multi-Hop Question Answering With Large Language Models Through Knowledge Graphs
  **作者**：Ahmmad O. M. Saleh, Gokhan Tur, Yucel Saygin
  **年份**：2024
  **出处**：Proceedings of ICNLSP 2024 (7th International Conference on Natural Language and Speech Processing)
  **链接**：论文PDF (ACL Anthology)
  **推荐理由**：该文提出 SubGraph RAG (SG-RAG) 方法，通过根据问题构造 Cypher 查询，从知识图谱中检索相关子图并转化为三元组文本作为 LLM 上下文，以回答多跳问题。研究表明相较于常规 RAG，SG-RAG 在多跳问答中能显著提高准确率，对比无检索或单纯向量检索的 LLM 答案准确度更高。该方法利用知识图谱结构信息增强检索，直接体现了结构化知识与 LLM 融合的思路，适用于需要复杂推理的智能问答场景。
- **标题**：Retrieval-Augmented Generation with Graphs (GraphRAG)
  **作者**：Haoyu Han 等（多作者）
  **年份**：2025
  **出处**：arXiv 预印本（未发表论文）
  **链接**：arXiv:2501.00309
  **推荐理由**：该论文系统综述了 GraphRAG 研究，提出了统一的 GraphRAG 框架，定义了查询处理、检索器、组织者、生成器等关键组件，并针对不同领域知识图的特点评述了各类 GraphRAG 技术。作为第一篇专门讨论“图结构+RAG”方法的综述，它总结了融合结构化图谱与非结构化检索的核心思路和挑战，对理解知识图谱增强检索生成的全貌、把握前沿方法具有重要参考价值。
- **标题**：Query Routing for Retrieval-Augmented Language Models
  **作者**：Jiarui Zhang, Xiangyu Liu, Yong Hu, Chaoyue Niu, Fan Wu, Guihai Chen
  **年份**：2025
  **出处**：arXiv 预印本
  **链接**：arXiv:2505.23052
  **推荐理由**：该文针对多模型 RAG 场景提出 RAGRouter 路由方法，利用文档嵌入和 RAG 能力嵌入进行对比学习来捕捉知识注入后模型能力的动态变化，使得路由决策可以感知检索结果对不同 LLM 的影响。实验证明 RAGRouter 在各知识密集型任务上比单一 LLM 或传统静态路由方案平均提升 3.29%–9.33% 的准确度。该工作关注“动态路由”在检索增强生成系统中的设计与效果，对多模型并行应用时如何智能选择最合适 LLM 的问题提供了新思路，与查询路由机制密切相关。
- **标题**：HybridRAG: Integrating Knowledge Graphs and Vector Retrieval Augmented Generation for Efficient Information Extraction
  **作者**：Bhaskarjit Sarmah, Benika Hall, Rohan Rao, Sunil Patel, Stefano Pasquali, Dhagash Mehta
  **年份**：2024
  **出处**：arXiv 预印本
  **链接**：arXiv:2408.04948
  **推荐理由**：该文首次提出将基于向量检索的 RAG（VectorRAG）和基于图检索的 RAG（GraphRAG）相结合的混合方法 HybridRAG，用于从金融报告等非结构化文档中抽取信息。实验结果显示，HybridRAG 同时利用向量数据库和知识图检索的上下文，在检索准确率和生成质量上均优于单独使用 VectorRAG 或 GraphRAG。该研究演示了结构化知识（图）与非结构化检索的互补优势，为工业级智能问答系统融合两者检索提供了设计范式。
- **标题**：SkewRoute: Training-Free LLM Routing for Knowledge Graph Retrieval-Augmented Generation via Score Skewness of Retrieved Context
  **作者**：Hairu Wang, Yuan Feng, Yukun Cao, Xike Xie, S. Kevin Zhou
  **年份**：2025
  **出处**：Findings of ACL: EMNLP 2025 (会议论文集)
  **链接**：ACL Anthology
  **推荐理由**：该文关注带有知识图检索的 RAG 场景中的路由问题，提出无需训练的 SkewRoute 框架。它发现检索结果得分分布的偏斜程度与问题难度高度相关，利用这一统计特征进行简单路由判断。实验证明与现有方法相比，SkewRoute 在性能-开销权衡上表现卓越，在保持或提升路由效果的同时显著降低了计算成本（路由效率提升 >3×，推理开销降低 >1000×）。该工作结合了知识图检索环境下的动态路由思想，提供了轻量级的路由机制，为多LLM集成的RAG系统设计提供了新视角。


