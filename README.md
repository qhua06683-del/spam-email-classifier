# 自动化邮件垃圾分类系统 (Spam Email Classifier)

## 📌 项目概述
本项目是一个基于 Python 实现的端到端文本挖掘与分类系统。通过对 5,572 条短信语料进行深度建模，系统能够精准识别垃圾邮件（Spam）与正常邮件（Ham）。项目严格遵循标准的数据挖掘流，引入了高级自然语言处理（NLP）流水线，并在稀疏特征空间下完成了多模型的横向对比与性能持久化。

---

## 🛠️ 技术栈
* **编程语言**：Python 3.x
* **核心工具库**：Scikit-learn (模型训练与评估), NLTK (自然语言处理), Pandas / NumPy (数据清洗)
* **文本特征工程**：TF-IDF (词频-逆文档频率) 向量化 
* **核心算法**：支持向量机 (Linear SVM)、朴素贝叶斯 (Naive Bayes)、逻辑回归 (Logistic Regression) 

---

## 📁 文件结构说明
```text
├── spam.csv                 # 原始短信语料数据集 (5572条)
├── source code/             # 源代码目录
├── confusion matrix.png     # 性能评估混淆矩阵热力图
├── final_spam_model.pkl     # 经优化训练完成的 SVM 预测引擎（序列化文件）
└── final_vectorizer.pkl     # 配套的文本特征提取与向量化工具（序列化文件）
