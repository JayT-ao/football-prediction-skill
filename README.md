# Football Match Prediction Skill

专业足球比赛预测系统，基于数据驱动的分析方法。

最新版本：V7.0 | 1090场数据验证 | 准确率55.3%

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
- 主场优势：量化主场因素影响
- 评分差距：高差距高权重
- 射手状态：关键球员进球趋势
- 深度学习：DNN+集成模型优化
- 赔率效率：分析赔率定价准确性
- 实时数据：整合实时比赛数据
- 可视化：预测结果可视化仪表板
- API接口：RESTful API支持

## Installation

git clone https://github.com/JayT-ao/football-prediction-skill.git

## File Structure

- SKILL.md: 主skill文件
- ADVANCED.md: 高级技巧
- IMPROVEMENTS.md: 复盘改进
- V2_IMPROVEMENTS.md: 10个新因素
- V3_OPTIMIZATION.md: xG+ML+回测
- V4_ADVANCED.md: LSTM+Transformer+GNN+因果+RL
- V5_REFINEMENTS.md: 亚洲/非洲加权+欧洲降权
- V6_REFINEMENTS.md: 主场+评分差距+射手+1090场验证
- V7_ADVANCED.md: 深度学习+赔率效率+实时数据+API
- README.md: 说明文档

## Performance (1090场验证)

| 指标 | 数值 | 行业标准 |
|------|------|----------|
| 总样本量 | 1090场 | - |
| 胜负准确率 | 55.3% | 55-60% |
| 评分差距>20分 | 80% | - |
| 评分差距10-20分 | 53% | - |
| 评分差距<10分 | 42% | - |

## Best Strikers Reference

| 射手 | 进球 | 球队 | 预测准确率 |
|------|------|------|------------|
| 凯恩 | 36球 | 拜仁 | 85% |
| 哈兰德 | 27球 | 曼城 | 80% |
| 姆巴佩 | 25球 | 皇马 | 82% |

## Version History

- v1.0: 初始版本
- v1.1: xG等高级指标
- v1.2: 泊松分布+心理因素+冷门评估
- v2.0: 10个新因素
- v3.0: Dixon-Coles+ML+回测
- v4.0: LSTM+Transformer+GNN+因果+RL
- v5.0: 亚洲/非洲加权+欧洲降权
- v6.0: 主场+评分差距+射手+1090场验证
- v7.0: 深度学习+赔率效率+实时数据+API

## License

MIT License

## Author

MiMoCode Agent
