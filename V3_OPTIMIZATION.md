# Football Prediction V3 Optimization

## Phase 1: Data Sources Expansion

### 1.1 xG Data (Understat)
- Source: understat.com
- Metrics: xG, xA, xT, shot quality

### 1.2 Advanced Stats (FBref)
- Source: fbref.com
- Metrics: Possession, PPDA, Key passes, Big chances

### 1.3 Injury Data (Transfermarkt)
- Source: transfermarkt.com
- Metrics: Current injuries, Return dates, Fitness

### 1.4 Head-to-Head Data
- Source: soccerway.com
- Metrics: Last 10 meetings, Goals, Home/Away record

---

## Phase 2: Model Improvements

### 2.1 Dixon-Coles Model
改进泊松分布，考虑进球相关性。

原理：
- 泊松分布假设进球独立
- 实际比赛中0-0和1-1比泊松预测更常见
- Dixon-Coles引入相关参数rho

### 2.2 Bayesian Update
贝叶斯更新，赛前实时调整。

公式：
P(H|E) = P(E|H) * P(H) / P(E)

调整因素：
- 伤病消息：5%
- 阵容变化：3%
- 天气变化：2%
- 赔率变化：4%

### 2.3 Monte Carlo Simulation
蒙特卡洛模拟，大量模拟取概率分布。

模拟次数：10000次
输出：
- 胜平负概率
- 各比分概率分布

---

## Phase 3: Machine Learning

### 3.1 Feature Engineering
特征列表：
- rating_diff：球队评分差
- attack_diff：进攻能力差
- defense_diff：防守能力差
- xg_diff：xG差
- xga_diff：xGA差
- form_diff：状态差
- home_advantage：主场优势
- odds_implied_prob：赔率隐含概率
- h2h_win_rate：历史交锋胜率

### 3.2 Models
- Logistic Regression
- Random Forest
- XGBoost
- Ensemble (加权平均)

权重：
- Logistic Regression: 30%
- Random Forest: 30%
- XGBoost: 40%

---

## Phase 4: Backtesting

### 4.1 Framework
- 输入：历史数据
- 输出：准确率、ROI、Sharpe Ratio

### 4.2 Metrics
- Overall accuracy
- Home/Draw/Away accuracy
- ROI (Return on Investment)
- Sharpe Ratio
- Brier Score

### 4.3 Optimization
- Grid Search
- Cross Validation
- Parameter Tuning

---

## V3 Prediction Function

输入：
- team_a, team_b：球队数据
- match_info：比赛信息

处理流程：
1. 获取xG数据
2. 获取H2H数据
3. 获取伤病数据
4. 获取天气数据
5. 获取裁判数据
6. 构建特征
7. Dixon-Coles模型
8. 蒙特卡洛模拟
9. 机器学习预测
10. 贝叶斯更新
11. 综合所有因素

输出：
- probabilities：胜平负概率
- top_scores：最可能比分
- features：特征值
- confidence：置信度

---

## Version History

### v3.0 (2026-06-20)
- Phase 1: 数据源扩展
- Phase 2: 模型改进
- Phase 3: 机器学习
- Phase 4: 回测验证