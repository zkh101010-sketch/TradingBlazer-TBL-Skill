# TradingBlazer-TBL-Skill
TBL language skill repository for Trading Blazer, including reusable tools, risk control modules and strategy templates to improve the quality of AI-generated quantitative strategies.
TradingBlazer-TBL-Skill/  # 仓库根目录（建议命名清晰，包含关键词TBL/TradingBlazer）
├── README.md              # 仓库核心说明（AI友好关键）
├── LICENSE                # 开源协议（可选，个人使用可选择MIT）
├── docs/                  # 文档目录（补充说明、AI使用指南、TBL语法参考）
│   ├── ai_prompt_template.md  # AI提示词模板（提升生成质量核心）
│   ├── tbl_syntax_cheat_sheet.md  # TBL语法速查
│   └── module_explanation.md     # 各模块功能详解
├── src/                   # 核心TBL代码目录（按功能拆分）
│   ├── utils/             # 通用工具函数（基础技能，AI高频调用）
│   │   ├── date_time_utils.tbl   # 日期时间处理（如K线周期转换、节假日判断）
│   │   ├── math_utils.tbl        # 数学计算（如移动平均、标准差、归一化）
│   │   └── risk_calc_utils.tbl   # 风险计算（如保证金、盈亏比）
│   ├── risk_control/      # 风险控制模块（核心策略技能）
│   │   ├── stop_loss_profit.tbl  # 止损止盈（固定点位、移动止损、百分比止损）
│   │   ├── position_management.tbl  # 仓位管理（固定仓位、凯利公式、动态仓位）
│   │   └── max_drawdown_control.tbl  # 最大回撤控制
│   ├── indicators/        # 自定义技术指标（扩展TBL内置指标）
│   │   ├── ma_cross_improve.tbl  # 改良均线交叉（如过滤假信号）
│   │   ├── rsi_advanced.tbl      # 高级RSI（如多周期共振、背离判断）
│   │   └── volume_indicator.tbl  # 量能指标（如成交量均线、量比）
│   └── strategy_templates/ # 完整策略模板（可直接修改参数使用）
│       ├── trend_following_template.tbl  # 趋势跟踪策略模板
│       ├── mean_reversion_template.tbl   # 均值回归策略模板
│       └── multi_factor_template.tbl     # 多因子策略模板
└── examples/              # 可运行的示例（验证skill可用性，AI参考案例）
    ├── simple_ma_strategy.tbl  # 基于utils+indicators的简单均线策略
    └── full_risk_control_strategy.tbl  # 完整带风险控制的趋势策略
