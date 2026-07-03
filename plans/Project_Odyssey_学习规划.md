# Project Odyssey — 两个月学习规划（~560 小时）

> **适用对象**：应用统计学研一，有理论基础但缺乏实践经验
> **目标岗位**：数据分析/机器学习/运筹优化方向实习
> **时间预算**：8 周 × 7 天 × 10 小时 = 约 560 小时
> **起始日期**：2026-07-03

---

## 一、你的画像与核心策略

### 当前状态

| 维度 | 水平 |
|------|------|
| 数学/统计 | 学过，复习可捡回 |
| Python 编码 | 能写简单脚本，不熟悉库，不会项目管理 |
| SQL | **零基础** |
| 机器学习/sklearn | 能跟着教程跑 demo，不能独立完成完整流程 |
| 深度学习/PyTorch | 书本级了解，零实战 |
| 运筹优化 | 课程学过，Python 未实现过 |
| Jupyter / Git / IDE / GitHub | 几乎不会 |
| 英语 | 中文资料为主 + 翻译辅助 |
| 硬件 | 无 GPU，可使用 Colab 免费版 |
| 每日可用时间 | 10 小时，可持续高强度 |
| 学习偏好 | 视频课 + 教材 + 项目实战 |
| 求职目标 | 尚未定向，全面探索后决定 |

### 核心原则

1. **以项目驱动主线**：每阶段有一个中心项目，技能为项目服务
2. **工具够用就行**：调包/IDE/Git 等工具类内容尽快通过，腾时间给算法
3. **算法三段式**：理解原理 → 手写推导 → 代码实现，不做调包侠
4. **2/8 法则**：用 20% 时间掌握 80% 实战场景
5. **SQL 持续练习**：每天 30 分钟 SQL 刷题，贯穿 8 周

---

## 二、每日时间模板

| 时段 | 时长 | 内容 | 说明 |
|------|------|------|------|
| 8:00-11:00 | 3h | **上午：理论学习** | 看视频/书籍，记笔记，理解概念 |
| 11:00-13:00 | 2h | 🔄 休息/运动/午餐 |
| 13:00-16:30 | 3.5h | **下午：编码实践** | 敲代码，跑通教程，完成当天练习 |
| 16:30-18:30 | 2h | 🔄 休息/运动/晚餐 |
| 18:30-22:00 | 3.5h | **晚上：项目推进** | 综合练习 + 30 分钟 SQL + 整理笔记 |

> 每周日晚上 20:00-22:00 为本阶段总结复盘时间。

---

## 三、八周详细规划

> **总原则**：工具/调包类 → 够用就行，尽快进入算法核心；
> 算法类 → 理解原理 + 手写推导 + 代码实现三段式；
> SQL → 每天 30 分钟不间断，贯穿全程。

---

### 第 1 周：Python 工程化 + SQL 起步（7/3 - 7/9）

> **核心目标**：工具链就位 + pandas 成为肌肉记忆 + SQL 基本查询

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| Git/GitHub + VSCode + Jupyter + venv | 1.5天 | 三个工具一次性贯通：创建 GitHub 仓库 → VSCode 打开 → 创建虚拟环境 → 用 Jupyter Notebook 写第一段分析代码 → git commit & push。**不分开学，一气呵成** |
| pandas 核心 | 2天 | Series/DataFrame 基础 → groupby/agg/transform → merge/concat → apply/map → 缺失值/重复值/异常值处理 → 时间序列类型 `datetime` 处理。**每个操作都闭卷练到不需要查文档** |
| matplotlib + seaborn | 0.5天 | 只学高频图：折线图、柱状图、散点图、热力图、分布图。**够画 EDA 报告就行** |
| SQL 入门 | 1.5天 | 《SQL 必知必会》通读 + SQLite 本地练习：SELECT/JOIN/GROUP BY/子查询/聚合函数/CASE WHEN |
| 本周项目 | 1.5天 | **电商销售数据 EDA**（[Kaggle Superstore](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting) 或 [和鲸社区](https://www.heywhale.com/) 中文版） |

#### 本周项目任务

1. GitHub 创建仓库，完整项目结构（`data/`, `notebooks/`, `src/`, `README.md`）
2. pandas 读入 → 清洗 → 聚合计算核心指标（月度销售额、利润率、地区分布）
3. 可视化输出 5-8 张图
4. 用 `pandasql` 或 SQLite 练习 SQL 查询同一份数据
5. 最终输出：一份完整的 Jupyter Notebook EDA 报告

#### 检查点

- [ ] GitHub 上有至少 1 个结构完整的仓库
- [ ] pandas groupby/merge/apply 能闭卷写
- [ ] SQL SELECT/JOIN/GROUP BY 能闭卷写
- [ ] EDA 项目完成并上传

---

### 第 2 周：SQL 进阶 + ML 实战 + 时序起手（7/10 - 7/16）

> **核心目标**：SQL 到窗口函数级别；独立完成 ML 建模流程；**提前启动时间序列**

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| SQL 进阶 | 2天 | 窗口函数 (ROW_NUMBER/RANK/LAG/LEAD) → CTE → CASE WHEN 复杂逻辑 → GROUPING SETS → 索引概念。LeetCode + 牛客网刷题 30+ |
| sklearn 快速回顾 | 0.5天 | **只做一遍完整流程回顾**：Pipeline → ColumnTransformer → 交叉验证 → GridSearchCV。不重学 API，直接用项目驱动 |
| 特征工程 | 1天 | 编码（One-Hot/Label/Target）→ 标准化/归一化 → 缺失值策略 → 特征选择（方差/相关性/重要性）→ 特征构造（组合特征、分箱）。**重中之重，不是调包** |
| XGBoost + LightGBM | 1天 | XGBoost 原理（Boosting 思想、正则化、并行化）→ 调参顺序（先树结构再学习率再采样）→ 特征重要性分析 → 过拟合诊断 |
| ⭐ **时间序列基础** | 1.5天 | **提前 1 周启动**：平稳性（ADF 检验）、趋势/季节性分解（STL）、ACF/PACF 图解读 → ARIMA 模型手动选参 (p,d,q) → statsmodels 跑通 |
| 本周项目 | 1天 | **客户流失预测** + **时序数据初探** |

#### 本周项目任务（两部分）

**A. ML 分类任务** — [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

1. SQL 做聚合探索（各维度流失率）
2. 特征工程 → Logistic Regression → Random Forest → XGBoost 逐步迭代
3. 对比 AUC、准确率、召回率，输出特征重要性排名
4. 代码写成 `.py` 脚本（不只是 Notebook）

**B. 时序热身** — [Air Passengers](https://www.statsmodels.org/stable/datasets/index.html) 经典数据集

5. 时间序列基本 EDA（趋势、季节分解、ADF 检验）
6. 手选 p/d/q 跑一个 ARIMA

#### 检查点

- [ ] SQL 窗口函数能闭卷写
- [ ] 不看教程，独立完成 ML 建模全流程
- [ ] 能解释 ACF/PACF 图在说什么
- [ ] 能手选 p/d/q 并解释为什么

---

### 第 3 周：时间序列深度 + 运筹优化起手（7/17 - 7/23）

> **核心目标**：时间序列成为一个能打的技能点；运筹优化开始理论复习

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| ARIMA/SARIMA 深入 | 1天 | 季节性 ARIMA → auto_arima 原理（不是单纯调包，要理解 AIC/BIC 选模逻辑）→ SARIMAX（加入外生变量） |
| Prophet | 1天 | 模型结构（趋势 + 季节 + 节假日 + 变点）→ 傅里叶级数 → 不确定性区间 → 交叉验证与调参 |
| 时序特征工程 + ML 时序 | 1.5天 | 滞后特征/滑动窗口/滚动统计 → 日历特征（节假日、工作日、月初月末）→ XGBoost/LightGBM 做时序（纯特征工程的威力） |
| 时序模型评估 | 0.5天 | 时间序列交叉验证（TimeSeriesSplit）、回测（Backtesting）→ MAPE/sMAPE/MASE 指标选择 |
| ⭐ **运筹优化理论复习** | 1.5天 | 线性规划回顾：标准型 → 单纯形法（手算一个例子）→ 对偶理论（影子价格的经济含义）→ 灵敏度分析。**用纸笔推导，不用代码** |
| 本周项目 | 1.5天 | **超市销量预测** + **LP 手算练习** |

#### 本周项目任务

1. 超市销量数据（[Walmart Sales](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting)）：趋势分解 → ADF 检验 → ACF/PACF
2. ARIMA 基线 → Prophet（加节假日）→ XGBoost 时序 → 三模型对比
3. 用 TimeSeriesSplit 做回测，输出 MAPE 对比表
4. **OR 练习**：做 3 道经典 LP 建模题（生产计划/运输问题/资源分配），纸笔写出数学模型

#### 检查点

- [ ] 能独立完成 ARIMA 建模全流程并解释每一步
- [ ] Prophet 能解释趋势变点检测原理
- [ ] 能手写一道线性规划的数学模型（决策变量/约束/目标函数）
- [ ] 理解影子价格的经济含义

---

### 第 4 周：PyTorch 从零到训练（7/24 - 7/30）

> **核心目标**：PyTorch 不再是书本概念，能写训练循环、DataLoader、自定义模型

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| DL 基础快速复习 | 0.5天 | 3Blue1Brown 视频 → 前向传播/反向传播/梯度下降/链式法则 → 激活函数 → 损失函数 → **用 numpy 手写一个单层网络的反向传播** |
| PyTorch 核心 | 3天 | Tensor 操作（广播、索引、设备切换）→ Autograd 机制（`requires_grad`, `backward()`, 计算图）→ `nn.Module` 自定义模型 → Dataset/DataLoader → **手写训练循环**（train/val loop, optimizer, loss, metrics） |
| MLP + CNN 简介 | 1.5天 | MLP 实战（隐藏层/激活函数/正则化）→ CNN 卷积/池化原理了解（不做重点）→ BatchNorm/Dropout |
| Colab GPU | 0.5天 | Colab 免费版使用 → 上传数据 → GPU 训练 → 保存/加载模型 |
| 本周项目 | 1.5天 | **房价预测：XGBoost vs MLP** |

#### 本周项目任务

1. [House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)：XGBoost 基线
2. PyTorch 搭建 MLP（至少 2 层隐藏层）做同一任务
3. 对比：训练速度 / 预测精度 / 可解释性
4. Colab GPU 上训练，记录加速比
5. 输出一份对比报告

#### 检查点

- [ ] 手写 PyTorch 训练循环，一次跑通不报错
- [ ] 理解 `model.train()` vs `model.eval()` vs `torch.no_grad()` 的区别
- [ ] 能用 DataLoader 高效加载数据
- [ ] Colab GPU 训练成功

---

### 第 5 周：LSTM + 序列深度学习（7/31 - 8/6）

> **核心目标**：LSTM 从原理到代码都能搞定；应用到时序多步预测

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| RNN/LSTM 原理 | 1.5天 | RNN 为何梯度消失 → **LSTM 三个门（遗忘门/输入门/输出门）逐行推导** → GRU 简化版 → [Colah's Blog](https://colah.github.io/posts/2015-08-Understanding-LSTMs/) 必读 |
| LSTM for 时序 | 2天 | 序列转监督学习（sliding window）→ 单步预测 → 多步预测（递归 vs 直接）→ Seq2Seq 结构（Encoder-Decoder）→ Teacher Forcing |
| 训练技巧 | 1天 | Early Stopping → LR Scheduler（ReduceLROnPlateau/Cosine）→ Gradient Clipping → Dropout → 权重初始化 → 过拟合诊断与应对 |
| 回顾巩固 | 1天 | 重写第 4 周 MLP + 本周 LSTM 训练循环，确保不查资料能写 |
| 本周项目 | 1.5天 | **电力消耗多步预测** |

#### 本周项目任务

1. [Household Power Consumption](https://www.kaggle.com/datasets/uciml/electric-power-consumption-data-set)：数据量大，练习序列处理
2. LSTM 单步 → LSTM 多步（预测未来 24h）→ Seq2Seq 多步
3. 对比：LSTM vs XGBoost 时序 vs ARIMA
4. Colab GPU 训练，记录实验过程

#### 检查点

- [ ] 能手绘 LSTM 三个门结构并解释
- [ ] 实现 LSTM 多步预测（至少两种策略）
- [ ] 能诊断过拟合并采取应对措施

---

### 第 6 周：Attention + Transformer + 现代时序（8/7 - 8/13）

> **核心目标**：理解并实现 Attention，掌握 Transformer 在时序中的应用

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| Attention 机制 | 1.5天 | **从零推导**：Query/Key/Value → Scaled Dot-Product Attention → Multi-Head Attention → Cross vs Self Attention → **手写一个 Attention 层的 PyTorch 实现** |
| Transformer | 1.5天 | [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) 精读 → Positional Encoding → Encoder/Decoder 结构 → LayerNorm vs BatchNorm → 为什么 Transformer 替代 LSTM |
| Time Series Transformer + TFT | 1.5天 | 时序中的 Transformer → TFT (Temporal Fusion Transformer) 核心思想（变量选择网络、门控机制、分位数输出）→ 用 PyTorch Forecasting 跑一个 TFT |
| 开源时序框架 | 0.5天 | darts / NeuralProphet / pytorch-forecasting 对比，会用其中一个 |
| 本周项目 | 2天 | ⭐ **需求预测综合实战 — 模型大比武** |

#### 本周项目任务

1. [M5 Competition](https://www.kaggle.com/competitions/m5-forecasting-accuracy) 或 [Store Item Demand](https://www.kaggle.com/c/demand-forecasting-kernels-only)
2. 同一数据集跑 **5 个模型**：ARIMA → Prophet → LSTM → Transformer → LightGBM
3. 模型集成（加权平均 / Stacking）
4. 输出完整对比报告（含训练时间、参数量、预测精度）
5. **这个项目是你的旗舰作品，做到能放到简历最显眼的位置**

#### 检查点

- [ ] 能手写 Scaled Dot-Product Attention 的 PyTorch 代码
- [ ] 能解释 Positional Encoding 为什么用 sin/cos
- [ ] 理解 Transformer vs LSTM 的核心差异
- [ ] 完成 5 模型对比项目

---

### 第 7 周：运筹优化深度实战（8/14 - 8/20）

> **核心目标**：Python 实现优化模型，打通"预测 → 优化"完整链路

| 模块 | 时间 | 核心内容 |
|------|------|----------|
| Python LP 建模 | 1.5天 | PuLP 上手（定义变量/约束/目标/求解/提取结果）→ cvxpy 了解 → **不仅是调包，要学会读求解器输出、诊断不可行/无界** |
| 整数规划 & MIP | 1.5天 | 0-1 变量建模（选址、指派问题）→ 大 M 法 → 分支定界思想 → 手建 3 个 MIP 模型 |
| 启发式算法 | 1.5天 | 遗传算法原理（编码/选择/交叉/变异）→ 模拟退火（温度衰减/接受概率）→ **不用现成库，手写 GA 解决一个简单优化问题** → 理解何时需要启发式 |
| 预测+优化全链路 | 1.5天 | 用第 6 周预测结果作为输入 → 建立优化模型 → 确定性优化 vs 随机规划简介 |
| 本周项目 | 1天 | ⭐ **供应链库存优化** |

#### 本周项目任务

1. **预测端**：用第 6 周最优模型预测各商品需求
2. **优化端**：基于预测值建库存模型（PuLP）
   - 决策变量：订货量、安全库存水平
   - 约束：预算、仓储容量、供应商 MOQ
   - 目标：最小化（订货成本 + 持有成本 + 缺货成本）
3. 敏感度分析：预测误差 ±10% 对最优策略的影响
4. GitHub README 写清问题背景、模型公式、求解结果

#### 检查点

- [ ] 能用 PuLP 独立建模求解 LP/MIP
- [ ] 能手写遗传算法解决简单优化问题
- [ ] 理解预测不确定性如何影响优化决策
- [ ] 完成预测+优化完整项目

---

### 第 8 周：收网 — 面试 + 简历 + 查漏补缺（8/21 - 8/27）

> **核心目标**：学的东西能讲出来，项目能亮出来，简历能投出去

| 模块 | 时间 | 内容 |
|------|------|------|
| SQL 面试冲刺 | 1天 | 牛客网/LeetCode 高频 SQL 集中刷，窗口函数 + 复杂业务查询 |
| ML/DL 面试知识 | 1.5天 | 整理面试高频问题清单：偏差-方差、过拟合方案、L1/L2 区别、XGBoost vs LightGBM、LSTM vs Transformer、Attention 原理 — **每个问题准备 2 分钟口述回答** |
| 时间序列面试 | 0.5天 | 平稳性、ACF/PACF、ARIMA 选参、Prophet 原理、多步预测策略 |
| 运筹优化面试 | 0.5天 | LP 标准型、对偶理论、MIP、启发式算法思想 |
| 简历撰写 | 1天 | 6 个项目包装：STAR 法则（情境-任务-行动-结果），每个项目 3-4 行 |
| GitHub 收尾 | 0.5天 | 每个仓库加完整 README（背景/方法/结果截图/如何运行） |
| 模拟面试 | 1天 | 找同学或自己录音：自我介绍 → 项目介绍 → 技术问答 |
| 查漏补缺 | 1天 | 模拟面试暴露的弱点集中修补 |

---

## 四、六阶段项目路线图

| 周 | 项目 | 核心技能 | GitHub 价值 |
|------|------|------|------|
| 1 | 电商数据 EDA | pandas, matplotlib, SQL, Git | ★★☆ |
| 2 | 客户流失预测 + 时序初探 | XGBoost, 特征工程, ARIMA 初探 | ★★★ |
| 3 | 超市销量预测 + LP 手算 | ARIMA, Prophet, LP 建模 | ★★★ |
| 4 | 房价预测：ML vs DL | PyTorch, MLP, Colab | ★★★ |
| 5 | 电力多步预测 | LSTM, Seq2Seq, 多步预测 | ★★★★ |
| 6 | ⭐ 需求预测五模型大比武 | Transformer, TFT, 模型集成 | ★★★★★ |
| 7 | ⭐ 供应链库存优化（预测+OR） | PuLP, MIP, GA, 全链路 | ★★★★★ |
| 8 | 简历 + 面试准备 | 6 项目完整包装 | — |

---

## 五、推荐的免费学习资源汇总

### Python & 工具链

| 资源 | 链接 | 用途 |
|------|------|------|
| 利用 Python 进行数据分析（第二版） | 豆瓣搜索 | pandas 圣经 |
| 黑马程序员 Python | B站搜索 | Python 基础补漏 |
| 廖雪峰 Python 教程 | liaoxuefeng.com | 快速查阅 |
| Git 入门教程 | B站搜索"Git 入门" | Git 基础 |
| VSCode 官方文档 | code.visualstudio.com/docs | IDE 使用 |

### SQL

| 资源 | 链接 | 用途 |
|------|------|------|
| SQL 必知必会 | 豆瓣/微信读书 | SQL 入门最快路径 |
| LeetCode 数据库题库 | leetcode.cn | 刷题 |
| 牛客网 SQL 实战 | nowcoder.com | 中文刷题 |

### 机器学习 & 深度学习

| 资源 | 链接 | 用途 |
|------|------|------|
| 动手学深度学习 (d2l.ai) | zh.d2l.ai | PyTorch 入门最佳教材 |
| scikit-learn 官方文档 | scikit-learn.org | API 参考 |
| 吴恩达 Machine Learning (2022) | Coursera | ML 理论（可加速看） |
| 3Blue1Brown 神经网络 | YouTube/B站 | 直观理解 DL |
| Colah's Blog — Understanding LSTM | colah.github.io | LSTM 经典文章 |
| The Illustrated Transformer | jalammar.github.io | Transformer 必读 |

### 时间序列

| 资源 | 链接 | 用途 |
|------|------|------|
| Forecasting: Principles and Practice (3e) | otexts.com/fpp3/ | 时序圣经，免费 |
| Kaggle Time Series Course | kaggle.com/learn | 快速上手 |
| Prophet 官方文档 | facebook.github.io/prophet/ | Prophet 实战 |

### 运筹优化

| 资源 | 链接 | 用途 |
|------|------|------|
| 王树尧 — 运筹学 | B站搜索 | 理论复习 |
| PuLP 官方文档 | coin-or.github.io/pulp/ | 实战建模 |
| cvxpy 官方文档 | cvxpy.org | 凸优化建模 |

---

## 六、重要提醒

### ⚠️ 预期管理

1. **这个规划非常激进**，几乎覆盖了一个数据科学硕士 1-2 年的核心课程。2 个月能做到的是：**每个模块都能跑通、能讲清楚、能放进简历**，但深度一定不够。
2. **如果目标是实习面试**，第 8 周前完成 6 个项目（每个仓库有 README + Notebook + 脚本），这比理论深度更有竞争力。
3. 如果中途某个模块卡住了 3 天以上，**跳过继续前进**，不要因为一个点拖慢整体进度。

### 🎯 方向优先级建议

虽然你想全面探索后再决定方向，但考虑到 2 个月有限：

- **优先攻克**：SQL、pandas、XGBoost/LightGBM、时序预测 — 覆盖 80% 数分/算法实习岗位
- **次优先**：PyTorch 深度学习、Transformer
- **如有余力**：运筹优化（小众但高壁垒方向）

### 📌 每日坚持习惯

- 每天用 **Markdown** 写学习笔记
- 每天至少 **git commit** 一次
- 每天 **30 分钟 SQL 刷题**，雷打不动
- 每周日晚上写周总结
- 遇到报错先自己 Debug 30 分钟再查资料

---

## 七、对比旧版的核心变化

| 内容 | 旧版 | 新版 | 原因 |
|------|------|------|------|
| sklearn | 2 天 | 0.5 天 | 你已能跟教程跑 demo，只需快速回顾 |
| 可视化 | 1 天 | 0.5 天 | 够画 EDA 图就行，不深入 |
| Git/VSCode/Jupyter | 分开 1.5 天 | 合并 1.5 天 | 一气呵成效率更高 |
| 时间序列 | 第 3 周才开始 | **第 2 周就起手** | 提前 1 周，多 1.5 天 |
| 运筹优化理论 | 第 7 周 | **第 3 周开始** | 提前复习 LP 理论，第 7 周专注代码 |
| 运筹优化总时长 | 6 天 | **7 天** | 增加了手写 GA + MIP 深度 |
| 启发式算法 | 调现成库 | **手写 GA** | 不用现成库，理解底层 |
| ML : DL : OR 比重 | 约 4:3:1 | 约 **3:4:2** | 减少调包 ML，增加算法深度 |
