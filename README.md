# 基于 MacBERT 微调的中文新闻分类模型 (Chinese News Classification Models based on Mac BERT)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

本项目基于Hugging Face的`macbert-base-chinese`模型，使用自定义的中文新闻数据集进行微调，构建了报道类型、报道框架和情感倾向三个用于新闻分类的深度学习模型。

This project leverages the `macbert-base-chinese` model from Hugging Face and fine-tunes it on a custom Chinese news dataset to build three deep learning models for news classification.


## 📦 模型概览 (Models Overview)

我们训练了三个不同的模型，具体信息如下：

| 模型名称 (Model Name) | 基于模型 (Base Model)        | 数据集 (Dataset)     | 
| --------------------- | ---------------------------- | ---------------------- |
| `[News-type]` | `hfl/macbert-base-chinese` | `[type_labeled]` |
| `[News-frame]` | `hfl/macbert-base-chinese` | `[frame_labeled]` |
| `[News-senti]` | `hfl/macbert-base-chinese` | `[senti-labeled]` | 

## 📊 性能表现 (Performance)

在测试集上的表现如下：

| 模型 (Model)                   | 准确率 (Accuracy) | 精确率 (Precision) | 召回率 (Recall) | F1分数 (F1-Score) |
| ------------------------------ | ----------------- | ------------------ | --------------- | ----------------- |
| `[News-type]`                  | `[0.89]`    | `[0.84]`     | `[0.82]`  | `[0.83]`    |
| `[News-frame]`                  | `[0.86]`    | `[0.85]`     | `[0.85]`  | `[0.85]`    |
| `[News-senti]`                  | `[0.81]`    | `[0.81]`     | `[0.87]`  | `[0.81]`    |
