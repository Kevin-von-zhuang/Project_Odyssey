# Project Odyssey — 56 天每日任务清单

> **时间模板**：上午 8:00-11:00（3h 理论）｜下午 13:00-16:30（3.5h 编码）｜晚上 18:30-22:00（3.5h 项目+SQL+笔记）
> **每日必修**：晚上 30 分钟 SQL 刷题 + git commit 一次 + Markdown 笔记 5 行
> **起始日**：2026 年 7 月 3 日（星期四）

---

## 第 1 周：Python 工程化 + SQL 起步（7/3 - 7/9）

### Day 1 — 7/3（周四）：工具链起手

**上午**
- [ ] 注册 GitHub 账号，了解 GitHub 是什么、为什么用
- [ ] 看 B站 Git 入门教程（前半部分：Git 原理、仓库概念、commit/push/pull）
- [ ] 了解 VSCode 界面：文件浏览器、终端、插件市场、命令面板（Ctrl+Shift+P）

**下午**
- [x] 确认 Python 3.8+ 已安装，检查 `python --version`
- [x] 安装 Git（git-scm.com），检查 `git --version`
- [ ] 在 GitHub 网页上创建仓库 `project-odyssey-eda`
- [ ] `git clone` 到本地，用 VSCode 打开该文件夹
- [x] 安装 VSCode 必装插件：Python、Jupyter、GitLens、Markdown Preview

**晚上**
- [x] 创建 Python 虚拟环境：`python -m venv venv` → 激活 → `pip install jupyter pandas matplotlib seaborn`
- [x] 在 VSCode 中创建第一个 Jupyter Notebook (`eda.ipynb`)
- [ ] 写第一个 cell：`print("Hello Odyssey")` 并运行
- [ ] 下载 Superstore 数据集 CSV 到 `data/` 文件夹
- [ ] `git add .` → `git commit -m "init project"` → `git push`
- [ ] 30 分钟 SQL：学习 SELECT、FROM、WHERE（《SQL 必知必会》第 2-4 章）
- [ ] Markdown 笔记：今天学会了什么？遇到什么坑？明天做什么？

---

### Day 2 — 7/4（周五）：pandas 深入（上）

**上午**
- [ ] 看《利用 Python 进行数据分析》第 4 章：NumPy 基础（数组、索引、广播、通用函数）
- [ ] 精读第 5 章前半：Series 和 DataFrame 的创建、索引、切片

**下午**
- [ ] 在 Jupyter Notebook 中逐个练习：
  - `pd.read_csv()` 读入 Superstore 数据
  - `.head()`, `.info()`, `.describe()`, `.shape`, `.columns`
  - `.iloc[]`, `.loc[]` 索引和切片
  - 布尔索引筛选数据
  - 新建列、删除列、重命名列
- [ ] 练习 `.value_counts()`, `.nunique()`, `.isnull().sum()`

**晚上**
- [ ] 继续 pandas 练习：`.sort_values()`, `.drop_duplicates()`
- [ ] 探索 Superstore 数据的缺失值和重复值并处理
- [ ] 30 分钟 SQL：学习 ORDER BY、LIMIT、LIKE、IN、BETWEEN（第 5 章）
- [ ] `git commit -m "day2 pandas basics"`
- [ ] Markdown 笔记

---

### Day 3 — 7/5（周六）：pandas 深入（下）

**上午**
- [ ] 精读第 5 章后半 + 第 6 章：数据载入、读写文件（CSV/Excel/JSON），`read_csv` 的常用参数
- [ ] 第 7 章：数据清洗和准备 — 缺失值处理（`dropna`, `fillna`）、重复值、数据转换（`map`, `replace`）

**下午**
- [ ] 练习 `.groupby()` + `.agg()` 组合拳（单列聚合、多列聚合、自定义聚合函数）
- [ ] 练习 `.transform()` 和 `.filter()`
- [ ] 练习 `pd.merge()`, `pd.concat()`（多表合并）
- [ ] 练习 `pd.cut()` / `pd.qcut()` 分箱
- [ ] 练习 `pd.to_datetime()`，从日期列提取年/月/日/星期

**晚上**
- [ ] 对 Superstore 数据做聚合分析：
  - 按地区、类别、月份分组计算销售额和利润
  - 找到利润率最高/最低的 10 个产品子类
- [ ] 30 分钟 SQL：聚合函数 COUNT/SUM/AVG/MAX/MIN + GROUP BY + HAVING（第 6-7 章）
- [ ] `git commit -m "day3 pandas advanced"`
- [ ] Markdown 笔记

---

### Day 4 — 7/6（周日）：可视化 + 周总结

**上午**
- [ ] 看 seaborn 官方 gallery，浏览所有图表类型，心中有数
- [ ] 精学 5 种核心图：
  - `sns.barplot()` — 柱状图（分类对比）
  - `sns.lineplot()` — 折线图（趋势）
  - `sns.scatterplot()` — 散点图（关系）
  - `sns.heatmap()` — 热力图（相关性）
  - `sns.histplot()` / `sns.boxplot()` — 分布图
- [ ] matplotlib 基础：`plt.subplots()`, `plt.title()`, `plt.xlabel()`, `plt.tight_layout()`

**下午**
- [ ] 用 Superstore 数据画 8 张图：
  1. 各产品类别销售额柱状图
  2. 月度销售额趋势折线图
  3. 销售额 vs 利润散点图
  4. 各地区销售额饼图/柱状图
  5. 利润率的箱线图
  6. 数值变量相关性热力图
  7. 各客户细分销售额对比
  8. Top 10 城市销售额排名
- [ ] 整理图表风格：统一配色、字体大小、图例位置

**晚上**
- [ ] **周总结复盘**（20:00-22:00）：
  - 回顾本周学到的所有 pandas/SQL/可视化操作
  - 哪些操作还需要查文档？（标记出来，明天起优先闭卷练习）
  - 本周项目 EDA 报告进度如何？
- [ ] 30 分钟 SQL：子查询（第 8 章）
- [ ] `git commit -m "day4 visualization"`
- [ ] Markdown 笔记

---

### Day 5 — 7/7（周一）：SQL 集中突破（上）

**上午**
- [ ] 通读《SQL 必知必会》第 9-11 章：子查询、联结表（INNER JOIN/LEFT JOIN/RIGHT JOIN）、自联结
- [ ] 理解 JOIN 的 Venn 图示，手画一遍各种 JOIN 的区别

**下午**
- [ ] 本地 SQLite 练习：
  - 创建数据库 `superstore.db`
  - 把 Superstore CSV 导入 SQLite
  - 用 pandas 的 `read_sql_query()` 执行 SQL
  - 练习 JOIN 查询：订单表 JOIN 退货表
- [ ] LeetCode SQL 刷题：3-5 道简单题（175, 176, 181, 182, 183）

**晚上**
- [ ] 继续 SQL 练习：写 5 个业务查询
  - 各地区的销售额和利润率
  - 每月的新客户数量
  - 每个产品类别的退货率
  - 高价值客户（消费金额 Top 20%）的购买特征
- [ ] 30 分钟 SQL：CASE WHEN 条件逻辑
- [ ] `git commit -m "day5 sql deep dive"`
- [ ] Markdown 笔记

---

### Day 6 — 7/8（周二）：SQL 集中突破（下）+ EDA 整合

**上午**
- [ ] 《SQL 必知必会》第 12-14 章：UNION、INSERT/UPDATE/DELETE、创建表
- [ ] 第 15-16 章：视图、存储过程概念（了解即可）
- [ ] 牛客网 SQL 实战：刷完 SQL 必知必会篇 10 题

**下午**
- [ ] 综合 SQL 练习：用 JOIN + GROUP BY + CASE WHEN + 子查询写 3 个复杂查询
- [ ] 练习将 SQL 查询结果直接导入 pandas DataFrame
- [ ] 补充 EDA 报告：在 Notebook 中加入 SQL 分析部分

**晚上**
- [ ] EDA 项目收尾整合：
  - 检查 Notebook 结构是否完整（开头介绍 → 数据概览 → 清洗过程 → 分析洞察 → 总结）
  - 补充每个图表的文字解读
  - 确保所有代码 cell 顺序正确、可以一次 Run All
- [ ] 30 分钟 SQL：复习本周所有 SQL 知识点，闭卷自测
- [ ] `git commit -m "day6 eda integration"`
- [ ] Markdown 笔记

---

### Day 7 — 7/9（周三）：EDA 项目完成 + 第 1 周收尾

**上午**
- [ ] EDA 项目最终检查：
  - 写 README.md（项目背景、数据来源、分析方法、关键发现）
  - 导出 Notebook 为 HTML 方便查看
- [ ] push 到 GitHub，确认仓库主页看起来专业

**下午**
- [ ] **闭卷自测（第 1 周核心技能）**：
  - pandas：groupby + agg、merge、apply、pivot_table
  - matplotlib/seaborn：5 种核心图
  - SQL：SELECT/JOIN/GROUP BY/子查询/CASE WHEN（各写 1 道题）
  - Git：clone → add → commit → push → pull 流程
- [ ] 标记仍不熟练的操作，纳入下周每天闭卷练习

**晚上**
- [ ] 预习第 2 周内容：浏览 XGBoost 官方文档目录、看看 Telco Customer Churn 数据集长什么样
- [ ] 30 分钟 SQL：LeetCode 刷 2 道新题
- [ ] `git commit -m "day7 week1 complete"`
- [ ] **周总结**：完成了什么？下周改进什么？

---

## 第 2 周：SQL 进阶 + ML 实战 + 时序起手（7/10 - 7/16）

### Day 8 — 7/10（周四）：SQL 进阶 — 窗口函数

**上午**
- [ ] 学习窗口函数概念：PARTITION BY vs GROUP BY 的区别
- [ ] 逐个掌握：
  - `ROW_NUMBER()` — 排名不跳号
  - `RANK()` — 排名跳号
  - `DENSE_RANK()` — 排名不跳号不间隔
  - `LAG()` / `LEAD()` — 前后行取值
  - `SUM() OVER()`, `AVG() OVER()` — 累积/移动聚合

**下午**
- [ ] LeetCode SQL 刷题（窗口函数专项）：176, 177, 178, 180, 184, 185
- [ ] 牛客网 SQL 进阶：窗口函数篇 10 题
- [ ] 在 Superstore 数据上练习：各品类销售额月度环比增长率（LAG）

**晚上**
- [ ] 综合窗口函数练习：写 3 个包含多窗口函数的复杂查询
- [ ] 复习本周要做的 ML 项目背景：客户流失预测是什么问题
- [ ] 30 分钟 SQL：CTE（WITH 子句）
- [ ] `git commit -m "day8 window functions"`
- [ ] Markdown 笔记

---

### Day 9 — 7/11（周五）：SQL 进阶 + sklearn 快速回顾

**上午**
- [ ] SQL 进阶收尾：CTE 递归、GROUPING SETS、索引概念
- [ ] LeetCode + 牛客网继续刷题，目标是 SQL 进阶题库存量达到 30+

**下午**
- [ ] **sklearn 快速回顾（0.5 天）**：
  - 不从头学 API，直接用一个简单数据集（Iris 或 Titanic）跑一遍：
    - `train_test_split` → `StandardScaler` → `OneHotEncoder`
    - `ColumnTransformer` → `Pipeline`
    - `LogisticRegression` → `cross_val_score` → `GridSearchCV`
    - `classification_report`, `confusion_matrix`
  - 这一遍跟教程可以，但要理解每一步在做什么

**晚上**
- [ ] 下载 Telco Customer Churn 数据集，做初步探索（`.info()`, 目标变量分布, 缺失值检查）
- [ ] 开始用 SQL 做客户流失数据的聚合分析
- [ ] 30 分钟 SQL：刷 3 道 LeetCode 中等题
- [ ] `git commit -m "day9 sklearn review + churn eda"`
- [ ] Markdown 笔记

---

### Day 10 — 7/12（周六）：特征工程

**上午**
- [ ] 系统学习特征工程（阅读 + 笔记）：
  - **数值型**：缺失值填充策略（均值/中位数/模型预测/KNN）、标准化（StandardScaler）vs 归一化（MinMaxScaler）的选择、分箱（equal-width vs equal-frequency）、对数/Box-Cox 变换
  - **分类型**：One-Hot Encoding、Label Encoding、Target Encoding（均值编码）、高基数类别处理（频率编码/embedding）
  - **特征构造**：组合特征、多项式特征、比率特征
  - **特征选择**：方差阈值、相关系数、单变量统计检验、模型特征重要性、递归特征消除（RFE）

**下午**
- [ ] 在 Churn 数据集上实践特征工程：
  - 分类型：One-Hot 编码低基数特征，Target Encoding 高基数特征
  - 数值型：标准化 + 缺失值处理
  - 构造 3-5 个新特征（如：总消费金额 / 合约月数）
  - 画相关性热力图，初步筛选特征

**晚上**
- [ ] Churn 数据继续处理：对目标变量 `Churn` 做 EDA，分析各特征与流失的关系
- [ ] 训练第一个基线模型：Logistic Regression
- [ ] 30 分钟 SQL：刷 3 道中等题
- [ ] `git commit -m "day10 feature engineering"`
- [ ] Markdown 笔记

---

### Day 11 — 7/13（周日）：XGBoost + LightGBM + 周总结

**上午**
- [ ] 学习 XGBoost 原理（不要只调包）：
  - Boosting 思想（串行、残差拟合）
  - XGBoost 的改进：二阶泰勒展开、正则化项、列采样、shrinkage
  - 核心参数：`n_estimators`, `max_depth`, `learning_rate`, `subsample`, `colsample_bytree`, `reg_alpha`, `reg_lambda`
  - 调参顺序：先固定学习率 0.1 → 调树的数量和深度 → 调采样参数 → 调正则化 → 降低学习率
- [ ] LightGBM vs XGBoost：Leaf-wise vs Level-wise、GOSS、EFB

**下午**
- [ ] Churn 数据集实战：Random Forest 基线 → XGBoost → LightGBM
- [ ] 画学习曲线（learning curve）和验证曲线（validation curve）
- [ ] 打印特征重要性排名，分析 Top 5 特征的业务含义
- [ ] 调参：用 GridSearchCV 或 Optuna 跑一轮

**晚上**
- [ ] **周总结复盘**（20:00-22:00）：
  - SQL 窗口函数能闭卷写吗？
  - sklearn 完整流程能独立跑通吗？
  - XGBoost 调参顺序记住了吗？
  - 这周 Churn 项目质量如何？哪里可以改进？
- [ ] 30 分钟 SQL：复习窗口函数 + CTE
- [ ] `git commit -m "day11 xgboost + weekly review"`
- [ ] Markdown 笔记

---

### Day 12 — 7/14（周一）：时间序列基础理论

**上午**
- [ ] 阅读 [Forecasting: Principles and Practice (3e)](https://otexts.com/fpp3/) 第 1-3 章：
  - 时间序列的组成部分：趋势（Trend）、季节性（Seasonality）、周期（Cycle）、残差（Residual）
  - 时间序列图形诊断
  - 简单预测方法：均值法、Naïve 法、季节性 Naïve 法、漂移法

**下午**
- [ ] 阅读第 4-5 章：
  - 平稳性（Stationarity）的定义和检验（ADF 检验 / KPSS 检验）
  - 差分（Differencing）消除趋势
  - 季节性差分
  - 单位根检验
- [ ] 下载 Air Passengers 数据集，做：
  - 趋势/季节分解（STL 分解 / `seasonal_decompose`）
  - ADF 检验，判断是否平稳
  - 画出 ACF 和 PACF 图

**晚上**
- [ ] 继续 Air Passengers 分析：
  - 解释 ACF/PACF 图的含义（截尾 vs 拖尾）
  - 尝试手动选出 p, d, q
- [ ] Churn 项目收尾：把 ML 部分代码整理成 `.py` 脚本
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day12 time series theory"`
- [ ] Markdown 笔记

---

### Day 13 — 7/15（周二）：ARIMA 实战

**上午**
- [ ] 阅读 FPP3 第 8-9 章：
  - ARIMA 模型详解：AR(p)、I(d)、MA(q) 各自含义
  - ACF/PACF 选参规则（AR 看 PACF 截尾，MA 看 ACF 截尾）
  - auto_arima 原理：AIC/BIC 如何选模
  - SARIMA：季节性参数 P/D/Q/m

**下午**
- [ ] Air Passengers 数据集：手工选 p/d/q → statsmodels ARIMA 拟合 → 诊断残差（Ljung-Box 检验、残差的 ACF）
- [ ] 用 `pmdarima.auto_arima` 自动选参，对比手工选参结果
- [ ] 训练集/测试集拆分 → 预测 → 评估（RMSE、MAE、MAPE）
- [ ] 画出预测值和真实值的对比图（含置信区间）

**晚上**
- [ ] 自己找一个新数据集（如月度气温、股票价格、网站流量等公开数据），独立跑一遍 ARIMA 全流程（不查教程）
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day13 arima practice"`
- [ ] Markdown 笔记

---

### Day 14 — 7/16（周三）：时序热身收尾 + ML 项目完成

**上午**
- [ ] 时序热身项目整合：
  - Air Passengers ARIMA 分析整理成 Notebook
  - 写清楚为什么选这个 p/d/q
  - 输出残差诊断图、预测图
- [ ] 如果时间充裕，尝试 SARIMA（加入季节性参数）

**下午**
- [ ] Churn 项目最终整合：
  - 代码从 Notebook 整理为清晰结构（`data/`, `src/`, `notebooks/`, `README.md`）
  - 写 README：项目背景 → 方法 → 结果（AUC 对比表）→ 关键发现（哪些特征最重要）
  - push 到 GitHub

**晚上**
- [ ] 预览第 3 周内容：看看 Walmart Sales 数据集，了解 Prophet 是什么
- [ ] 30 分钟 SQL：刷 3 道 LeetCode 中等题
- [ ] `git commit -m "day14 week2 complete"`
- [ ] Markdown 笔记

---

## 第 3 周：时间序列深度 + 运筹优化起手（7/17 - 7/23）

### Day 15 — 7/17（周四）：ARIMA/SARIMA 深入

**上午**
- [ ] SARIMA 深入：季节性阶数 P/D/Q/m 的选择逻辑
- [ ] SARIMAX：加入外生变量（如促销、节假日、天气）
- [ ] auto_arima 源码级理解：AIC 计算公式、搜索策略（stepwise vs 全搜索）
- [ ] 模型诊断：残差白噪声检验、正态性检验、残差相关性

**下午**
- [ ] 下载 Walmart Sales 数据集，做时序 EDA：
  - 多商店、多部门的销售量趋势
  - 季节性模式（按周、月、年）
  - 节假日效应（感恩节、圣诞节前后的销量变化）
- [ ] 选一个 Store-Department 组合，跑 ARIMA/SARIMA
- [ ] 尝试加入温度/油价等外生变量（如有）

**晚上**
- [ ] 继续 Walmart 建模：用 auto_arima 选参 + 残差诊断
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 16 — 7/18（周五）：Prophet 实战

**上午**
- [ ] 学习 Prophet 模型结构（读官方文档 + 论文 Abstract）：
  - 趋势模型：分段线性/逻辑增长 + 变点检测
  - 季节模型：傅里叶级数
  - 节假日效应：独立的高斯冲击
  - 不确定性区间：趋势模拟
- [ ] 理解 Prophet 与传统时序方法的根本区别（加法模型 vs ARIMA 的自回归结构）

**下午**
- [ ] Prophet 代码实战（Walmart 数据）：
  - 准备数据（`ds` 和 `y` 列）
  - 基础 Prophet 拟合 → 预测
  - 加入节假日（创建 holidays DataFrame）
  - 调参：`changepoint_prior_scale`, `seasonality_prior_scale`, `holidays_prior_scale`
  - 交叉验证：`cross_validation()` + `performance_metrics()`

**晚上**
- [ ] Prophet vs ARIMA 对比（同一数据）：
  - 画出两个模型的预测对比图
  - 计算 MAPE/RMSE 对比
  - 分析各自的优劣势
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 17 — 7/19（周六）：时序特征工程 + ML 时序

**上午**
- [ ] 系统学习时序特征工程：
  - **滞后特征**（Lag Features）：t-1, t-2, t-7, t-30, t-365
  - **窗口特征**（Rolling Features）：7 天均值、30 天标准差、7 天最大/最小值
  - **日历特征**：年、月、日、星期、是否周末、是否月初/月末、距某节假日的天数
  - **特殊特征**：同比值、环比增长率、累积值

**下午**
- [ ] Walmart 数据：构造 20+ 个时序特征
- [ ] 用 XGBoost/LightGBM 做时序预测（纯特征工程方法）：
  - 训练集/测试集按时间切分（不能用随机切！）
  - 训练 → 预测 → 评估
- [ ] 画出特征重要性，看哪些滞后/窗口特征最重要

**晚上**
- [ ] 三模型对比初稿：ARIMA / Prophet / XGBoost 时序
- [ ] 整理对比表格（模型、MAPE、训练时间、优点、缺点）
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 18 — 7/20（周日）：时序评估方法 + 周总结

**上午**
- [ ] 学习时间序列模型评估：
  - 为什么不能用随机 K-Fold CV？（时间序不可打乱）
  - TimeSeriesSplit（扩展窗口 / 滑动窗口）
  - 回测（Backtesting）方法论
  - 指标选择：MAPE / sMAPE / MASE / RMSE / MAE 各自的适用场景和缺陷

**下午**
- [ ] Walmart 项目完善：
  - 用 TimeSeriesSplit 正确做交叉验证
  - 重新计算三个模型的回测指标
  - 完善对比图表和文字分析
  - 整理代码结构

**晚上**
- [ ] **周总结复盘**（20:00-22:00）：
  - 时序三模型（ARIMA/Prophet/XGBoost）各自的适用场景？
  - 时序交叉验证为什么不能用 K-Fold？
  - Walmart 项目进展，下周收尾
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day18 week3 review"`
- [ ] Markdown 笔记

---

### Day 19 — 7/21（周一）：运筹优化理论 — LP 回顾

**上午**
- [ ] 打开运筹学教材或看 [B站王树尧运筹学](https://www.bilibili.com/)，复习：
  - 线性规划标准型（Standard Form）
  - 解的概念：可行解、最优解、顶点、基变量/非基变量
  - 单纯形法（Simplex Method）流程：进基 → 出基 → 旋转 → 迭代

**下午**
- [ ] **手算一个完整的单纯形法例子**（纸笔）：
  - 找一个 2 变量 3 约束的 LP 问题
  - 画出可行域（图形法验证）
  - 用单纯形法表格一步步算
  - 验证最优解

**晚上**
- [ ] 继续做 2 道 LP 手算题
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 20 — 7/22（周二）：对偶理论 + LP 建模

**上午**
- [ ] 学习对偶理论：
  - 原始问题 → 对偶问题的转换规则
  - 弱对偶性和强对偶性
  - **影子价格（Shadow Price）的经济含义**：每增加一单位资源，目标函数能改善多少
  - 互补松弛条件

**下午**
- [ ] **LP 建模练习（纸笔写出数学模型，不写代码）**：
  1. 生产计划问题：多产品、多资源约束，最大化利润
  2. 运输问题：多工厂、多仓库，最小化运输成本
  3. 资源分配问题：多项目、有限预算，最大化总收益
- [ ] 对每道题写出：决策变量定义 → 目标函数 → 所有约束条件

**晚上**
- [ ] 反思：如果用 Python 求解，需要什么工具？—— 预告 PuLP
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 21 — 7/23（周三）：模型评估收尾 + Walmart 完成

**上午**
- [ ] 时序模型评估方法复习 + 补充：
  - 预测区间（Prediction Interval）vs 置信区间（Confidence Interval）
  - 残差的异方差性检验
  - 模型稳定性的概念

**下午**
- [ ] **Walmart 项目最终整合**：
  - 三模型（ARIMA/Prophet/XGBoost 时序）完整对比
  - 写 README：项目背景 → 数据描述 → 方法 → 结果对比 → 结论
  - 代码整理为 `.py` 脚本 + Notebook
  - push 到 GitHub

**晚上**
- [ ] 预览第 4 周：3Blue1Brown 神经网络视频
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day21 week3 complete"`
- [ ] Markdown 笔记

---

## 第 4 周：PyTorch 从零到训练（7/24 - 7/30）

### Day 22 — 7/24（周四）：DL 基础复习 + NumPy 手写反向传播

**上午**
- [ ] 看 [3Blue1Brown 神经网络系列](https://www.youtube.com/watch?v=aircAruvnKk)（B站有搬运）：
  - 第 1 集：神经网络是什么
  - 第 2 集：梯度下降
  - 第 3 集：反向传播的直觉
- [ ] 复习关键概念：前向传播、损失函数（MSE、Cross-Entropy）、激活函数（ReLU、Sigmoid、Tanh）、梯度下降、链式法则

**下午**
- [ ] **用 NumPy 手写一个单隐藏层神经网络的反向传播**（这是理解 PyTorch 的关键）：
  - 前向传播：`X → W1 → ReLU → W2 → MSE Loss`
  - 反向传播：手推梯度 `∂Loss/∂W2`、`∂Loss/∂W1`
  - 用 NumPy 实现，不调任何 DL 库
  - 在简单数据集上验证（如 XOR 问题或 Iris）
- [ ] 把代码和推导过程整理到 Jupyter Notebook 中

**晚上**
- [ ] 安装 PyTorch：`pip install torch torchvision torchaudio`
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day22 numpy backprop"`
- [ ] Markdown 笔记

---

### Day 23 — 7/25（周五）：PyTorch Tensor + Autograd

**上午**
- [ ] 读 d2l.ai 第 3 章：Tensor 基础操作
  - 创建 Tensor、形状变换（reshape/view/unsqueeze/squeeze）
  - 索引和切片、广播机制
  - 设备切换（CPU ↔ GPU：`.to('cuda')` / `.to('cpu')`）
  - 数学运算、矩阵乘法（`@` / `mm` / `matmul`）
- [ ] 读第 4 章：Autograd 自动求导
  - `requires_grad=True` 的含义
  - `.backward()` 如何计算梯度
  - 计算图（Computation Graph）的构建与释放
  - `torch.no_grad()` 的使用场景
  - `grad.zero_()` 为什么每次都要清零

**下午**
- [ ] 在 Jupyter Notebook 中逐个实验：
  - 创建各种 Tensor，玩弄 reshape 和广播
  - 设置 `requires_grad=True`，做前向计算然后 `backward()`
  - 验证 Autograd 计算出的梯度与手算是否一致
  - 实验 `torch.no_grad()` 和不用的区别

**晚上**
- [ ] 用 PyTorch 的 Tensor + Autograd 重写昨天的 NumPy 反向传播
- [ ] 对比：PyTorch 版本简洁了多少？
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day23 pytorch tensor autograd"`
- [ ] Markdown 笔记

---

### Day 24 — 7/26（周六）：nn.Module + DataLoader

**上午**
- [ ] 读 d2l.ai 第 5 章：`nn.Module` 和模型构建
  - `nn.Linear`, `nn.ReLU`, `nn.Sigmoid`, `nn.Dropout`, `nn.BatchNorm1d`
  - `nn.Sequential` vs 自定义 `nn.Module` 类
  - `forward()` 方法的写法
  - 参数初始化：`nn.init` 各种方法
- [ ] 读第 6 章：数据处理
  - `TensorDataset` → `DataLoader`
  - `batch_size`, `shuffle`, `num_workers`
  - 自定义 `Dataset` 类（`__len__`, `__getitem__`）

**下午**
- [ ] 搭建第一个完整的 PyTorch MLP：
  - 自定义 `nn.Module` 类（2 层隐藏层）
  - 创建 DataLoader
  - 写训练循环：`for epoch in range(...):` 嵌套 `for X_batch, y_batch in dataloader:`
  - 记录 train loss / val loss
- [ ] 在 Iris 数据集上跑通

**晚上**
- [ ] 下载 House Prices 数据集，准备 PyTorch 格式
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day24 nn module dataloader"`
- [ ] Markdown 笔记

---

### Day 25 — 7/27（周日）：MLP + CNN 简介 + 周总结

**上午**
- [ ] 读 d2l.ai 第 7 章：MLP 深入
  - 隐藏层宽度和深度的选择
  - 激活函数的选择和比较
  - 过拟合与欠拟合在训练曲线上的表现
  - 权重衰减（L2 正则化）
- [ ] 读第 8 章：CNN 简介（了解概念，不做重点）
  - 卷积层、池化层、通道概念

**下午**
- [ ] House Prices 数据：搭建 MLP（3 层隐藏层，不同宽度）→ 训练 → 评估
- [ ] 实验：不同网络结构（宽度/深度）对效果的影响
- [ ] 实验：不同激活函数（ReLU/LeakyReLU/GELU）的区别

**晚上**
- [ ] **周总结复盘**（20:00-22:00）：
  - PyTorch 训练循环能闭卷写吗？
  - `model.train()` / `model.eval()` / `torch.no_grad()` 各自什么时候用？
  - Autograd 的原理理解了没？
  - House Prices MLP vs XGBoost 对比做得如何？
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day25 mlp cnn intro"`
- [ ] Markdown 笔记

---

### Day 26 — 7/28（周一）：Colab GPU + 训练实战

**上午**
- [ ] 学习 Google Colab 使用：
  - 注册 Google 账号，打开 Colab
  - 上传 Notebook、挂载 Google Drive
  - 切换 GPU 运行时（Runtime → Change runtime type → GPU）
  - 上传本地数据到 Colab
  - 保存模型到 Google Drive / 下载到本地

**下午**
- [ ] 把 House Prices MLP 项目迁移到 Colab：
  - 上传数据和 Notebook
  - 修改代码适配 Colab 路径
  - GPU 训练 → 记录训练时间
  - CPU 训练 → 记录训练时间
  - **记录加速比**

**晚上**
- [ ] 学习模型的保存和加载：
  - `torch.save(model.state_dict(), 'model.pth')`
  - `model.load_state_dict(torch.load('model.pth'))`
  - 保存完整模型 vs 保存参数的区别
  - 保存 checkpoint（含 optimizer 状态、epoch 信息）以便恢复训练
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 27 — 7/29（周二）：House Prices 项目深入

**上午**
- [ ] House Prices 项目优化：
  - 特征工程：用 sklearn 的 Pipeline 做预处理，再转 PyTorch Dataset
  - 尝试不同的网络架构（更宽 vs 更深）
  - 加入 Dropout 和 BatchNorm
  - 实验不同学习率（0.1, 0.01, 0.001, 0.0001）

**下午**
- [ ] MLP vs XGBoost 深度对比：
  - 相同训练集/测试集
  - 比较：RMSE、训练时间、推理时间、可解释性
  - 分析 MLP 在什么情况下超过 XGBoost、什么情况下不如

**晚上**
- [ ] 整理对比报告到 Notebook
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 28 — 7/30（周三）：第 4 周收尾

**上午**
- [ ] **闭卷自测（PyTorch 核心）**：
  - 手写训练循环（不查资料）
  - 手写自定义 `nn.Module` 类
  - 手写 DataLoader 创建过程
  - 手写模型保存/加载代码

**下午**
- [ ] House Prices 项目整合：
  - 整理代码结构（`src/model.py`, `src/train.py`, `src/data.py`）
  - 写 README（项目背景、ML vs DL 对比、结论、如何运行）
  - push 到 GitHub

**晚上**
- [ ] 预览第 5 周：看 Colah's Blog LSTM 文章（配合翻译）
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day28 week4 complete"`
- [ ] Markdown 笔记

---

## 第 5 周：LSTM + 序列深度学习（7/31 - 8/6）

### Day 29 — 7/31（周四）：RNN/LSTM 原理（上）

**上午**
- [ ] 学习 RNN 基础：
  - RNN 结构：隐藏状态、循环连接、时间展开（Unrolling）
  - 为什么 RNN 能处理序列：参数共享
  - RNN 的致命缺陷：梯度消失和梯度爆炸
  - BPTT（Backpropagation Through Time）

**下午**
- [ ] 学习 LSTM（精读）：
  - **[Colah's Blog](https://colah.github.io/posts/2015-08-Understanding-LSTMs/) 全文精读**（配合翻译）
  - 手绘 LSTM 结构图，标注三个门
  - 遗忘门（Forget Gate）：决定丢弃什么信息
  - 输入门（Input Gate）：决定存储什么新信息
  - 输出门（Output Gate）：决定输出什么信息
  - 细胞状态（Cell State）的更新公式

**晚上**
- [ ] 用 NumPy 手写一个简化版 LSTM 的前向传播（不需反向传播）
- [ ] 理解 LSTM 公式中每个变量的维度
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day29 rnn lstm theory"`
- [ ] Markdown 笔记

---

### Day 30 — 8/1（周五）：LSTM 原理（下）+ GRU

**上午**
- [ ] LSTM 公式逐行推导（纸笔）：
  - $f_t = \sigma(W_f \cdot [h_{t-1}, x_t] + b_f)$
  - $i_t = \sigma(W_i \cdot [h_{t-1}, x_t] + b_i)$
  - $\tilde{C}_t = \tanh(W_C \cdot [h_{t-1}, x_t] + b_C)$
  - $C_t = f_t * C_{t-1} + i_t * \tilde{C}_t$
  - $o_t = \sigma(W_o \cdot [h_{t-1}, x_t] + b_o)$
  - $h_t = o_t * \tanh(C_t)$
- [ ] GRU 简化版对比：重置门 + 更新门，为什么参数更少效率更高

**下午**
- [ ] PyTorch `nn.LSTM` 实战：
  - 理解 `input_size`, `hidden_size`, `num_layers` 参数
  - LSTM 的输入输出维度（`(seq_len, batch, input_size)` → `(seq_len, batch, hidden_size)`）
  - `output, (hidden, cell) = lstm(input)` 接收返回值
  - 用随机数据跑通一个 LSTM，确认维度正确

**晚上**
- [ ] 下载 Household Power Consumption 数据集，做初步探索
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 31 — 8/2（周六）：LSTM 时序预测（上）

**上午**
- [ ] 学习序列转监督学习（Sliding Window）：
  - 给定序列 $[x_1, x_2, ..., x_T]$，用前 $k$ 个值预测下一个值
  - 如何用 `timeseries_dataset_from_array` 或手动构建 window
  - 单步预测 vs 多步预测的区别

**下午**
- [ ] 电力数据：构建 sliding window 数据集
- [ ] 搭建 LSTM 单步预测模型 → 训练 → 评估
- [ ] 画出预测曲线 vs 真实曲线

**晚上**
- [ ] 单步预测优化：调隐藏层大小、层数、学习率
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 32 — 8/3（周日）：LSTM 多步预测 + 周总结

**上午**
- [ ] 学习多步预测策略：
  - **递归策略（Recursive）**：用预测值作为输入继续预测下一步 → 误差累积
  - **直接策略（Direct）**：训练多个模型，每个预测一个未来步 → 模型太多
  - **Seq2Seq/多输出策略**：一次性输出多个未来值 → 推荐方案

**下午**
- [ ] 电力数据：实现 LSTM 多步预测（预测未来 24 小时）
- [ ] 对比单步 vs 多步的误差（多步通常更大，为什么？）
- [ ] Seq2Seq 结构初探：Encoder LSTM → Decoder LSTM
- [ ] Teacher Forcing 的概念

**晚上**
- [ ] **周总结复盘**：
  - LSTM 三个门的作用能闭卷解释吗？
  - LSTM 公式能写出来吗？
  - 单步 vs 多步预测的误差差异原因？
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day32 lstm multistep"`
- [ ] Markdown 笔记

---

### Day 33 — 8/4（周一）：训练技巧

**上午**
- [ ] 系统学习 DL 训练技巧：
  - **Early Stopping**：监控 val loss，patience=N 后停止
  - **Learning Rate Scheduler**：ReduceLROnPlateau（val loss 不降时降低 LR）、Cosine Annealing、Warmup
  - **Gradient Clipping**：防止梯度爆炸
  - **权重初始化**：Xavier、Kaiming
  - **Dropout**：训练时随机丢弃神经元

**下午**
- [ ] 在电力数据 LSTM 上逐个实验：
  - 加 Early Stopping → 对比不加的效果
  - 加 ReduceLROnPlateau → 观察 LR 变化曲线
  - 加 Gradient Clipping → 观察梯度范数
  - 加 Dropout → 对比过拟合程度

**晚上**
- [ ] 整理实验记录：每个技巧对模型性能的影响
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 34 — 8/5（周二）：回顾巩固 + 电力项目整合

**上午**
- [ ] **闭卷重写**：不查资料，从头写一个 LSTM 多步预测项目
  - 数据处理（sliding window）
  - 模型定义（nn.Module）
  - 训练循环（含 Early Stopping、LR Scheduler）
  - 评估和可视化

**下午**
- [ ] 电力项目完整收尾：
  - LSTM vs XGBoost 时序 vs ARIMA（三模型对比）
  - 代码整理为脚本 + Notebook
  - 写 README

**晚上**
- [ ] 预览第 6 周：看 The Illustrated Transformer
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day34 lstm review + power project"`
- [ ] Markdown 笔记

---

### Day 35 — 8/6（周三）：过拟合诊断专题 + 第 5 周收尾

**上午**
- [ ] **过拟合 vs 欠拟合深度诊断**：
  - 训练误差远小于验证误差 → 过拟合
  - 训练误差和验证误差都很大 → 欠拟合
  - 应对过拟合：更多数据、Dropout、正则化、简化模型、数据增强
  - 应对欠拟合：更大模型、更长训练、降低正则化、更好的特征

**下午**
- [ ] 有意制造过拟合（小数据 + 大模型）→ 诊断 → 修复（加 Dropout/正则化）→ 观察变化
- [ ] 有意制造欠拟合（小模型 + 大数据）→ 诊断 → 修复（增大模型）→ 观察变化
- [ ] 整理成"过拟合诊断手册"笔记

**晚上**
- [ ] 第 5 周所有代码 push + 周报
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day35 week5 complete"`
- [ ] Markdown 笔记

---

## 第 6 周：Attention + Transformer + 现代时序（8/7 - 8/13）

### Day 36 — 8/7（周四）：Attention 机制（上）

**上午**
- [ ] 理解 Attention 的直觉：
  - 人类大脑如何"注意"：在阅读一个句子时，不同词之间的关联程度不同
  - 传统 Seq2Seq 的瓶颈：所有信息压缩到最后一个隐藏状态
  - Attention 的核心思想：动态加权求和

**下午**
- [ ] **从公式手推 Attention**：
  - Query、Key、Value 是什么？（通过线性变换从输入得到）
  - Attention Score：$score(Q, K) = QK^T$
  - Scaled Dot-Product：$Attention(Q, K, V) = softmax(\frac{QK^T}{\sqrt{d_k}})V$
  - **为什么除以 $\sqrt{d_k}$ ？**（防止点积过大导致 softmax 梯度消失）

**晚上**
- [ ] 用 NumPy 手写 Scaled Dot-Product Attention
- [ ] 在随机数据上验证维度变化
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day36 attention theory"`
- [ ] Markdown 笔记

---

### Day 37 — 8/8（周五）：Attention 机制（下）

**上午**
- [ ] Multi-Head Attention：
  - 多个注意力头并行工作，每个头关注不同方面，等价于多个"子空间"
  - 公式：$MultiHead(Q, K, V) = Concat(head_1, ..., head_h)W^O$
  - 每个 head 先做线性投影降维，再做 Attention
- [ ] Cross-Attention vs Self-Attention：
  - Self-Attention：Q、K、V 来自同一序列
  - Cross-Attention：Q 来自 Decoder，K、V 来自 Encoder

**下午**
- [ ] **用 PyTorch 手写一个 Multi-Head Attention 层**（继承 `nn.Module`）：
  - 实现 `__init__`（定义线性层 W_Q, W_K, W_V, W_O）
  - 实现 `forward`（计算 Q/K/V → 分头 → Scaled Dot-Product → Concat → 输出投影）
  - 在随机数据上测试维度正确性
- [ ] 对比 PyTorch 内置的 `nn.MultiheadAttention`，验证结果一致

**晚上**
- [ ] 开始读 [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day37 multihead attention code"`
- [ ] Markdown 笔记

---

### Day 38 — 8/9（周六）：Transformer 融合

**上午**
- [ ] The Illustrated Transformer 精读完毕：
  - Encoder 结构：Self-Attention → Add & Norm → FFN → Add & Norm
  - Decoder 结构：Masked Self-Attention → Cross-Attention → FFN
  - Positional Encoding：$PE(pos, 2i) = sin(pos / 10000^{2i/d})$，$PE(pos, 2i+1) = cos(pos / 10000^{2i/d})$
  - **为什么用 sin/cos？**（相对位置信息、可外推、无需学习）

**下午**
- [ ] 理解 LayerNorm vs BatchNorm：
  - BatchNorm：对一个 batch 内同一特征做归一化
  - LayerNorm：对一个样本内所有特征做归一化
  - 为什么 Transformer 用 LayerNorm？（序列长度可变、batch 内样本独立性）

**晚上**
- [ ] 理解 Transformer 为什么替代 LSTM：
  - 并行计算（不需要等上一个时间步）
  - 长距离依赖（Attention 直接连接任意两个位置）
  - 但 Attention 复杂度是 O(n²)（这是代价）
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day38 transformer fusion"`
- [ ] Markdown 笔记

---

### Day 39 — 8/10（周日）：时间序列 Transformer + 周总结

**上午**
- [ ] 学习时间序列中的 Transformer 应用：
  - Informer：通过 ProbSparse Self-Attention 降低复杂度
  - Autoformer：用自相关机制替代自注意力
  - 时间序列 Transformer 的核心难点：位置编码在长序列上的表现、计算复杂度

**下午**
- [ ] 学习 TFT (Temporal Fusion Transformer)：
  - 变量选择网络（Variable Selection Network）：自动学习哪些输入特征重要
  - 门控残差网络（Gated Residual Network）
  - 分位数输出（不只是一个点预测，而是预测分布）
  - 静态协变量 vs 时变协变量的处理

**晚上**
- [ ] **周总结复盘**：
  - Attention 公式能闭卷写吗？
  - Transformer 结构能画出来吗？
  - 为什么除以 √d_k？
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day39 time series transformer"`
- [ ] Markdown 笔记

---

### Day 40 — 8/11（周一）：PyTorch Forecasting + 开源框架

**上午**
- [ ] 学习 PyTorch Forecasting 框架：
  - `TimeSeriesDataSet` — 自动处理时序数据（静态/时变分类/时变连续变量）
  - `TemporalFusionTransformer.from_dataset()` — 一行代码创建 TFT
  - Trainer 训练 + 预测
  - 结果可视化（Attention 图、变量重要性）

**下午**
- [ ] 用 M5 Competition 数据（或简化版），跑一个 TFT：
  - 准备数据格式
  - 创建 `TimeSeriesDataSet`
  - 训练 TFT
  - 画出分位数预测（10%/50%/90%）
  - 画出变量重要性

**晚上**
- [ ] 浏览其他开源时序框架：darts、NeuralProphet 的基本用法
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 41 — 8/12（周二）：五模型大比武（上）

**上午**
- [ ] M5 或 Store Item Demand 数据准备：
  - 数据清洗、特征工程
  - 统一的训练集/测试集切分（确保所有模型用同一份数据）
  - 确定评估指标（RMSE、MAE、MAPE）

**下午**
- [ ] 跑通 3 个模型：
  - ARIMA/SARIMA（statsmodels）
  - Prophet（单一时间序列或分组）
  - LightGBM 时序（特征工程版本）

**晚上**
- [ ] 跑通剩余 2 个模型：
  - LSTM（PyTorch 手写版）
  - Transformer/TFT（PyTorch Forecasting）
- [ ] 记录每个模型的训练时间、预测时间、RMSE
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 42 — 8/13（周三）：五模型大比武（下）+ 旗舰项目完成

**上午**
- [ ] 模型集成（Ensemble）：
  - 简单加权平均
  - 学习权重（用 Linear Regression 学各模型权重）
  - Stacking（用元模型学习如何组合）
- [ ] 比较集成前后的效果提升

**下午**
- [ ] **旗舰项目整合** — 这是你的简历头牌：
  - 整理所有模型代码，统一接口
  - 画出 5 模型 + 集成的预测对比图（一张大图）
  - 对比表格（模型、RMSE、MAE、MAPE、训练时间、参数量、优点、缺点）
  - 关键洞察：哪个模型在什么场景下最好？为什么？
  - 写一篇高质量的 README（目标、方法、结果、结论、如何复现）

**晚上**
- [ ] push 到 GitHub，这是你的第 1 个五星项目 ⭐
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day42 flagship project complete"`
- [ ] Markdown 笔记

---

## 第 7 周：运筹优化深度实战（8/14 - 8/20）

### Day 43 — 8/14（周四）：Python LP 建模 — PuLP

**上午**
- [ ] 安装 PuLP + CBC 求解器：`pip install pulp`
- [ ] 读 PuLP 官方文档 Quick Start：
  - `LpProblem`：创建问题（最大化/最小化）
  - `LpVariable`：定义决策变量（连续/整数/0-1、上下界）
  - `lpSum`：线性和表达式
  - `+=`：添加目标函数和约束
  - `solve()`：求解
  - `.value()` / `.varValue`：提取结果

**下午**
- [ ] 用 PuLP 求解第 3 周手算的 3 道 LP 题：
  1. 生产计划问题
  2. 运输问题
  3. 资源分配问题
- [ ] 对比手算结果和代码结果
- [ ] 学习读求解器输出：Optimal / Infeasible / Unbounded — 各自如何处理

**晚上**
- [ ] 自创一道 LP 题（结合实际场景），建模并求解
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 44 — 8/15（周五）：整数规划 & MIP

**上午**
- [ ] 学习整数规划（Integer Programming / MIP）：
  - LP 解是连续值，实际中很多变量必须是整数（人、台、个）
  - 0-1 变量的强大：可以建模"是/否"、"开/关"、"选/不选"
  - 分支定界法（Branch and Bound）基本原理

**下午**
- [ ] MIP 建模实战：
  1. **选址问题（Facility Location）**：选哪些仓库位置，最小化建设成本 + 运输成本
  2. **背包问题（Knapsack）**：选哪些物品，不超过容量，价值最大
  3. **指派问题（Assignment）**：工人分配给任务，一个工人一个任务，总成本最小
- [ ] 每题都用 PuLP 求解（关键是用 0-1 变量建模）

**晚上**
- [ ] 大 M 法（Big-M Method）建模逻辑：如何用 MIP 建模 if-then 逻辑约束
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 45 — 8/16（周六）：启发式算法 — 遗传算法手写

**上午**
- [ ] 学习遗传算法（Genetic Algorithm）原理：
  - **编码（Encoding）**：如何把解表示成染色体（二进制/实数/排列）
  - **初始种群（Population）**：随机生成一组解
  - **适应度（Fitness）**：评估每个解的好坏
  - **选择（Selection）**：轮盘赌选择、锦标赛选择
  - **交叉（Crossover）**：单点交叉、两点交叉、均匀交叉
  - **变异（Mutation）**：随机扰动，保持多样性
  - **终止条件**：达到最大代数 / 适应度收敛

**下午**
- [ ] **手写遗传算法（不调用现成 GA 库）**：
  - 选一个简单优化问题（如 TSP 旅行商问题 / 0-1 背包 / 函数优化）
  - 从零实现编码 → 适应度 → 选择 → 交叉 → 变异 → 迭代
  - 画出适应度随代数的收敛曲线

**晚上**
- [ ] 对比 GA 解 vs PuLP 精确解（小规模问题验证 GA 正确性，大规模问题观察 GA 优势）
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day45 genetic algorithm from scratch"`
- [ ] Markdown 笔记

---

### Day 46 — 8/17（周日）：模拟退火 + 启发式 vs 精确方法 + 周总结

**上午**
- [ ] 学习模拟退火（Simulated Annealing）原理：
  - 温度（Temperature）：高 → 接受差解概率大（探索），低 → 接受差解概率小（利用）
  - 退火调度（Cooling Schedule）：温度如何衰减
  - Metropolis 准则：$P(accept\ worse) = e^{-\Delta E / T}$
  - 与遗传算法的对比：SA 是单点搜索，GA 是种群搜索

**下午**
- [ ] 手写模拟退火解决同一个问题
- [ ] 对比启发式方法 vs 精确方法的场景：
  - 小规模（< 50 变量）→ 精确方法（LP/MIP）最优
  - 大规模（> 1000 变量）→ 启发式方法可行
  - 非线性/非凸 → 必须用启发式

**晚上**
- [ ] **周总结复盘**：
  - PuLP 能独立建模了吗？
  - GA 的五个步骤能闭卷写吗？
  - 什么时候用精确方法、什么时候用启发式？
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 47 — 8/18（周一）：预测+优化全链路（上）

**上午**
- [ ] 回顾第 6 周预测模型成果，选定最优秀的时序模型
- [ ] 设计优化场景：
  - 某电商/零售商有 N 种商品
  - 已知未来 7 天各商品预测需求量（从时序模型来）和预测误差分布
  - 需要决定：每种商品订多少货？
  - 约束：总预算 B 元、仓库容量 V 立方米、供应商最低起订量 MOQ
  - 目标：最小化（订货成本 + 仓储成本 + 缺货损失成本）

**下午**
- [ ] 建数学模型（纸笔 + LaTeX）：
  - 决策变量：$x_i$（商品 i 的订货量）
  - 约束：$\sum p_i x_i \le B$（预算），$\sum v_i x_i \le V$（容量），$x_i \ge MOQ_i$ 或 $x_i = 0$（MOQ）
  - 目标：$\min \sum(c_i x_i + h_i \mathbb{E}[\max(x_i - d_i, 0)] + s_i \mathbb{E}[\max(d_i - x_i, 0)])$
  - 这是随机优化！需要处理需求 $d_i$ 的不确定性

**晚上**
- [ ] 学习两种处理不确定性的方法：
  - **确定性等价模型**：用预测均值代替随机变量（最简单，但忽略了不确定性）
  - **随机规划简介**：Scenario-based（生成多个需求场景，最小化期望成本）
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 48 — 8/19（周二）：全链路项目实现

**上午**
- [ ] 生成模拟数据（基于第 6 周预测结果构造需求分布）：
  - 预测均值 → 作为需求分布的均值
  - 预测标准差 → 用 Prophet 的不确定性区间或 LSTM 分位数预测
- [ ] 确定性模型 PuLP 实现（使用预测均值）

**下午**
- [ ] 场景随机规划实现：
  - 生成 100 个需求场景（从分布中抽样）
  - 建 MIP 模型（订货量用 0-1 变量处理 MOQ 约束）
  - 求解期望成本最小化
- [ ] 对比确定性方案 vs 随机方案的成本差异

**晚上**
- [ ] 敏感度分析：
  - 需求预测误差 ±10% → 最优策略如何变化？总成本增加多少？
  - 预算增加 20% → 总成本降低多少？
  - 哪个约束是最紧的瓶颈？
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 49 — 8/20（周三）：全链路项目整合 + 第 7 周收尾

**上午**
- [ ] 整合预测+优化全链路项目：
  - `data/` — 原始数据和生成数据
  - `src/forecast.py` — 预测模型
  - `src/optimize.py` — 优化模型
  - `notebooks/analysis.ipynb` — 完整分析流程
  - `README.md` — 项目说明

**下午**
- [ ] README 重点突出：
  - 业务问题描述（零售商库存管理）
  - 技术方案（预测+优化的全链路架构）
  - 模型公式（用 LaTeX 在 README 中展示）
  - 求解结果（最优订货策略可视化）
  - 敏感度分析结论
  - 如何运行代码

**晚上**
- [ ] push 到 GitHub — 这是你的第 2 个五星项目 ⭐
- [ ] 30 分钟 SQL
- [ ] `git commit -m "day49 week7 complete OR pipeline"`
- [ ] Markdown 笔记

---

## 第 8 周：收网 — 面试 + 简历 + 查漏补缺（8/21 - 8/27）

### Day 50 — 8/21（周四）：SQL 面试冲刺

**上午**
- [ ] 牛客网 SQL 实战：集中刷 15 道高频题，重点：
  - 窗口函数（排名、移动平均、同比环比）
  - 复杂 JOIN（多表、自联结）
  - CASE WHEN 条件分组
  - CTE + 子查询嵌套

**下午**
- [ ] LeetCode SQL 中等题集中攻克 10 道
- [ ] 整理"SQL 常见面试问题"清单，每题写出标准答案

**晚上**
- [ ] SQL 闭卷自测：随机 3 道 LeetCode 中等题，计时完成
- [ ] `git commit -m "day50 sql sprint"`
- [ ] Markdown 笔记

---

### Day 51 — 8/22（周五）：ML/DL 面试知识整理

**上午**
- [ ] **ML 面试高频问题清单**（逐题写出 2 分钟口述回答）：
  1. 偏差（Bias）和方差（Variance）的权衡
  2. L1 正则化和 L2 正则化的区别（公式 + 为什么 L1 产生稀疏解）
  3. XGBoost vs LightGBM 的区别，各自优缺点
  4. 特征重要性的计算方法有哪些
  5. 如何处理类别不平衡（过采样/欠采样/SMOTE/代价敏感）
  6. 交叉验证的作用和常见策略
  7. 过拟合的检测方法和应对策略
  8. 特征工程的常见方法
  9. AUC-ROC 的含义和计算
  10. Bagging vs Boosting 的区别

**下午**
- [ ] **DL 面试高频问题清单**：
  1. 反向传播的原理（链式法则）
  2. 梯度消失和梯度爆炸的原因和解决方案
  3. BatchNorm 的原理和作用
  4. Dropout 的原理（为什么相当于集成学习）
  5. Adam 优化器的原理（Momentum + RMSProp）
  6. 为什么 Transformer 取代 LSTM
  7. Attention 的公式和含义
  8. `model.train()` vs `model.eval()` 的区别
  9. 迁移学习（Transfer Learning）的概念
  10. 多 GPU 训练的基本策略（DataParallel / DistributedDataParallel）

**晚上**
- [ ] 录音自测：每道题录下自己的回答，听一遍，改进
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 52 — 8/23（周六）：时序 + 运筹面试知识 + 项目故事

**上午**
- [ ] **时间序列面试高频问题**：
  1. 什么是平稳性？如何检验？不平稳怎么办？
  2. ACF 和 PACF 的区别，如何用它们选 ARIMA 参数
  3. ARIMA(p,d,q) 三个参数的含义
  4. Prophet 和 ARIMA 的本质区别
  5. 多步预测的几种策略及优缺点
  6. 时序交叉验证为什么不能用普通 K-Fold
  7. LSTM vs Transformer 在时序上的对比

**下午**
- [ ] **运筹优化面试高频问题**：
  1. 线性规划的标准型和基本定理
  2. 对偶理论和影子价格的经济含义
  3. LP 和 MIP 的区别，MIP 为什么比 LP 难
  4. 什么是 NP-Hard，什么情况要用启发式
  5. 遗传算法的基本流程
- [ ] **STAR 法则准备项目故事**：每个项目准备 3 分钟口述
  - 情境（S）：业务背景是什么
  - 任务（T）：我需要解决什么问题
  - 行动（A）：我用了什么技术、做了什么分析
  - 结果（R）：效果如何、学到什么

**晚上**
- [ ] 练习完整的自我介绍（1 分钟版本 + 3 分钟版本）
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 53 — 8/24（周日）：简历撰写

**上午**
- [ ] 列出简历框架：
  - 教育背景（学校、专业、GPA（如果不差的话）、相关课程）
  - 技能清单（分类：编程语言/数据分析/机器学习/深度学习/运筹优化/工具）
  - 项目经历（6 个项目）
  - 实习/竞赛/其他经历（如有）

**下午**
- [ ] **项目经历撰写（STAR 法则 × 6 个项目）**：
  1. ⭐ 供应链需求预测五模型大比武
  2. ⭐ 供应链库存优化（预测+优化全链路）
  3. 电力消耗多步预测（LSTM + Seq2Seq）
  4. 超市销量预测（ARIMA + Prophet + XGBoost）
  5. 客户流失预测（XGBoost + 特征工程）
  6. 电商销售数据 EDA

- [ ] 每个项目 3-4 行，突出：技术栈、量化结果、业务价值

**晚上**
- [ ] 简历格式化（LaTeX / 超级简历 / Canva），生成 PDF
- [ ] 找人 review（同学/学长/导师）
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 54 — 8/25（周一）：GitHub 收尾

**上午**
- [ ] 逐个仓库检查 README：
  - 项目背景（一句话说清楚）
  - 数据来源
  - 技术方法（用了什么模型/算法）
  - 主要结果（关键图表截图、数据）
  - 如何运行（`git clone` → `pip install -r requirements.txt` → `python src/main.py`）
  - 项目亮点（2-3 条 bullet point）

**下午**
- [ ] 每个仓库补充 `requirements.txt`（`pip freeze > requirements.txt`）
- [ ] 每个仓库补充 `.gitignore`（Python 模板）
- [ ] 每个仓库补充代码注释（关键函数和类）
- [ ] GitHub 个人主页完善：头像、Bio、Pinned repositories（Pin 住最重要的 6 个项目）

**晚上**
- [ ] 确保所有仓库的 commit 历史干净、有意义（不要有一堆 "update" 提交）
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 55 — 8/26（周二）：模拟面试

**上午**
- [ ] 完整模拟面试流程（自己录音或找同学）：
  - 1 分钟自我介绍
  - 项目深度追问（为什么选这个模型？遇到过什么困难？怎么解决的？）
  - 技术问答（ML/DL/时序/OR 各抽 2 题）
  - SQL 现场写题（LeetCode 中等难度一道）
  - 反问环节（你有什么想问我们的？）

**下午**
- [ ] 听录音，找出问题：
  - 哪里停顿太久？
  - 哪里解释不清楚？
  - 哪些技术问题答不上来？
  - 自我介绍是否吸引人？
- [ ] 针对性改进 + 重新录一遍

**晚上**
- [ ] 准备 3 个反问问题（体现你对公司和岗位的思考）
- [ ] 30 分钟 SQL
- [ ] `git commit`
- [ ] Markdown 笔记

---

### Day 56 — 8/27（周三）：最终查漏补缺 + 旅程结束

**上午**
- [ ] 根据模拟面试暴露的弱点，集中修补：
  - 某个算法原理还说不清楚？→ 重新推导一遍
  - 某个项目的技术细节模糊？→ 重新看一遍代码
  - 某个 SQL 题型还卡？→ 针对性再刷 5 题
  - 自我介绍不流畅？→ 再练 5 遍

**下午**
- [ ] **学习总结文档**：回顾 56 天的学习历程
  - 学会了哪些技能？（列清单）
  - 完成了哪些项目？（6 个项目链接）
  - 最大的收获是什么？
  - 之后还需要继续深化的方向？
- [ ] 整理学习笔记库，方便日后查阅

**晚上**
- [ ] 最后检查：
  - [ ] GitHub 主页整洁、6 个项目 README 完整
  - [ ] 简历 PDF 就绪
  - [ ] 面试知识清单随时可复习
  - [ ] LeetCode/牛客网 SQL 题量达标
- [ ] 🎉 **56 天 Odyssey 之旅完成！开始投递简历！**

---

## 附录：每日必修清单（打印贴在桌前）

- [ ] 上午 3h 理论学习（视频/书籍/笔记）
- [ ] 下午 3.5h 编码实践（不摆烂，敲每一个代码）
- [ ] 晚上 3.5h 项目推进
- [ ] 每天 30 分钟 SQL 刷题（雷打不动）
- [ ] 每天 `git commit` 至少一次
- [ ] 每天 5 行 Markdown 学习笔记
- [ ] 遇到 bug 先自己 debug 30 分钟
- [ ] 周日晚上 20:00-22:00 周总结复盘
