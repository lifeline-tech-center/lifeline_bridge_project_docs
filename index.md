---
layout: home
title: 🏗️ 生命线平台-桥梁专项模型开发文档
nav_order: 1
---

# 📚 生命线平台-桥梁专项技术文档索引

欢迎访问**城市生命线安全工程监测平台**相关的桥梁数据分析与预警模型说明文档。  
本文档涵盖以下两大类模块：

- [� 生命线平台-桥梁专项技术文档索引](#-生命线平台-桥梁专项技术文档索引)
  - [📊 数据分析方法](#-数据分析方法)
  - [🚨 预警模型](#-预警模型)
    - [🛠 开发中模块](#-开发中模块)

---

## 📊 数据分析方法

用于对桥梁结构响应数据进行处理、降维、特征提取与频谱分析等。

- [📈 特征分析-加速度信号分解模块（acc_eemd_decomposition）](./acc_eemd_decomposition/README.md)  
  ➤ 基于 EEMD 分解加速度信号以提取关键模态特征。

- [🔍 特征分析-PCA 特征降维模块（feature_analysis）](./feature_analysis/README.md)  
  ➤ 使用主成分分析（PCA）对高维传感器数据降维。

- [📊 加速度频谱分析模块（acc_spectral_analyse）](./acc_spectral_analyse/README.md)  
  ➤ 对桥梁加速度数据进行单通道频谱分析、多时段频谱分析、多设备频谱分析和滤波分析等。

- [🧠 自动模态频率识别模块（autossi）](./autossi/README.md)  
  ➤ 利用SSI和聚类算法自动提取模态频率。

- [🔗 相关性分析模块（correlation_analysis）](./correlation_analysis/README.md)  
  ➤ 分析结构响应与环境因素之间的相关性。

- [📊 统计分析模块（stats_analysis）](./stats_analysis/README.md)  
  ➤ 提供频率统计、概率拟合、最大值最小值等统计功能。

- [🧹 数据异常识别与处理模块（data_preprocessing）](./data_preprocessing/README.md)  
  ➤ 基于滑动中位数与 MAD 方法进行数据异常识别与插值处理。

- [📉 趋势分析模块（trend_analysis）](./trend_analysis/README.md)  
  ➤ 识别结构长期变化趋势，如应变漂移、挠度发展、频率衰减。

---

## 🚨 预警模型

用于实现关键结构指标的动态监测与预警。

- [🧱 支座脱空预警模块（bearing_alert）](./bearing_alert/README.md)  
  ➤ 判断支座反力变化是否超出正常范围，识别脱空风险。

- [📐 伸缩缝位移异常预警模块（joint_displacement_alert）](./joint_displacement_alert/README.md)  
  ➤ 基于温度-位移关系构建动态阈值模型，识别异常伸缩缝行为。

- [📉 模态频率下降预警模块（freq_alert）](./freq_alert/README.md)  
  ➤ 基于模态频率对比模型识别结构刚度降低迹象。

- [🏗️ 主梁持续下挠预警模块（progressive_deflection_alert）](./progressive_deflection_alert/README.md)  
  ➤ 利用时间序列趋势识别主梁下挠持续发展状态。

- [🧩 混凝土主梁裂缝超限预警模块（crack_detection_alert）](./crack_detection_alert/README.md)  
  ➤ 基于传感器反馈识别裂缝宽度/速度的异常增长。

---

### 🛠 开发中模块

- 🚛 超载预警模块（overload_alert）
- 🚢 船撞预警模块（ship_collision_alert）
- 🔄 主梁防倾覆预警模块（anti_overturning_alert）