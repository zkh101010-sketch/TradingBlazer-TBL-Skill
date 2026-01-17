# TradingBlazer-TBL-Skill
TBL language skill repository for Trading Blazer, including reusable tools, risk control modules and strategy templates to improve the quality of AI-generated quantitative strategies.
# TradingBlazer-TBL-Skill
TBL language skill repository for Trading Blazer, including reusable tools, risk control modules and strategy templates to improve the quality of AI-generated quantitative strategies.
## 📂 仓库目录结构
### 根目录
- `README.md`：仓库核心说明（AI友好关键）
- `LICENSE`：开源协议（可选，个人使用可选择MIT）
- `.gitignore`：Git忽略文件（过滤无用文件，如临时文件、日志）

### ref/（参考文档，用于需按需查阅的非代码类知识（架构、政策、细则、流程））
- `ai_prompt_template.md`：AI提示词模板（提升生成质量核心）
- `tbl_syntax_cheat_sheet.md`：TBL语法速查
- `module_explanation.md`：各模块功能详解

### src/（核心TBL代码用于需重复编写、要求确定性 / 可靠性的任务）
#### utils/（通用工具函数，AI高频调用）
- `date_time_utils.tbl`：日期时间处理（如K线周期转换、节假日判断）
- `math_utils.tbl`：数学计算（如移动平均、标准差、归一化）
- `risk_calc_utils.tbl`：风险计算（如保证金、盈亏比）

#### risk_control/（风险控制模块，核心策略技能）
- `stop_loss_profit.tbl`：止损止盈（固定点位、移动止损、百分比止损）
- `position_management.tbl`：仓位管理（固定仓位、凯利公式、动态仓位）
- `max_drawdown_control.tbl`：最大回撤控制

#### indicators/（自定义技术指标，扩展TBL内置指标）
- `ma_cross_improve.tbl`：改良均线交叉（如过滤假信号）
- `rsi_advanced.tbl`：高级RSI（如多周期共振、背离判断）
- `volume_indicator.tbl`：量能指标（如成交量均线、量比）

### assets/（可运行的示例，用于最终输出需要的模板（样板代码））
- `trend_following_template.tbl`：趋势跟踪策略模板
- `mean_reversion_template.tbl`：均值回归策略模板
- `multi_factor_template.tbl`：多因子策略模板
- `simple_ma_strategy.tbl`：基于utils+indicators的简单均线策略
- `full_risk_control_strategy.tbl`：完整带风险控制的趋势策略
