# Football Match Prediction Skill

专业足球比赛预测系统，基于数据驱动的分析方法。

## Features

- 数据驱动：基于ESPN实时数据、博彩赔率、球队统计
- 积分形势分析：考虑出线形势对比赛态度的影响
- 高级统计：xG、xA、PPDA等专业指标
- 概率估算：泊松分布、埃洛评分等数学模型
- 价值评估：计算EV值、凯利公式优化投注
- 串关策略：稳健/平衡/进取型方案
- 风险管理：资金管理、止损策略、心态控制
- 心理因素：考虑球队心理素质和比赛压力
- 冷门评估：独立评估冷门概率

## Installation

git clone https://github.com/JayT-ao/football-prediction-skill.git

## File Structure

- SKILL.md: 主skill文件，包含完整预测流程
- ADVANCED.md: 高级技巧，包含概率模型和机器学习方法
- IMPROVEMENTS.md: 基于实际比赛复盘的改进方案
- README.md: 说明文档

## Quick Start

触发关键词:
- 预测、分析
- 胜负、结果
- 比分、进球
- 串关、投注、买
- 价值、赔率、EV

预测流程:
1. 数据采集（ESPN赔率+球队数据）
2. 积分形势分析（出线形势+比赛态度）
3. 实力对比（进攻/防守/伤停/状态）
4. 概率估算（泊松分布+综合调整）
5. 价值评估（EV计算+价值筛选）
6. 串关策略（组合原则+类型选择）

## Advanced Features

### 高级统计指标
- xG（Expected Goals）：预期进球
- xA（Expected Assists）：预期助攻
- PPDA：逼抢强度
- 关键传球：创造力评估

### 概率模型
- 泊松分布：比分概率计算
- 埃洛评分：球队实力评估
- 布拉德利-特里模型：胜负概率

### 心理因素评估
- 必须赢的压力影响
- 已经出线的轮换风险
- 基本出局的无压力状态
- 生死战的破釜沉舟

### 冷门独立评估
- 实力差距分析
- 近期状态对比
- 历史交锋参考
- 综合冷门概率

## Risk Management

### 凯利公式
f = (bp - q) / b
f: 最优投注比例
b: 赔率 - 1
p: 胜率
q: 1 - p

建议使用半凯利或1/4凯利降低风险

### 资金管理
- 只用闲钱
- 设定预算
- 不要追损
- 分散投注

## Value Assessment

EV = (实际概率 x 赔率回报) - 100%

| EV值 | 建议 |
|------|------|
| 大于+30% | 强烈推荐 |
| +10%到+30% | 推荐 |
| +5%到+10% | 可以考虑 |
| 0%到+5% | 一般 |
| 小于0% | 不推荐 |

## Data Sources

- ESPN: 赛程、赔率、球队数据
- Understat: xG数据
- FBref: 综合数据
- Transfermarkt: 伤病信息

## Improvements (Based on Real Match Analysis)

### 发现的问题
- 进球数预测偏差+57%
- 胜负方向准确率50%
- 平局概率偏低
- 心理因素利用不足

### 改进方案
- 泊松分布进球预测
- 平局概率调整
- 心理因素评估
- 冷门独立评估

详见 IMPROVEMENTS.md

## License

MIT License

## Author

MiMoCode Agent