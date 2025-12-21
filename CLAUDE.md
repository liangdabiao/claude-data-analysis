# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Claude Data Analysis Assistant is an intelligent data analysis platform that leverages Claude Code's sub-agents, slash-commands, and hooks to provide a comprehensive data analysis workflow. Based on the successful DATAGEN multi-agent architecture, this project offers a modern, user-friendly interface for data analysis tasks.

## Quick Start

1. Place your data files in the `data_storage/` directory
2. Use `/analyze [filename]` to start data analysis
3. Use `/visualize [filename]` to create visualizations
4. Use `/report [filename]` to generate analysis reports

## Core Features

### Sub-Agents
- **data-explorer**: Data exploration and statistical analysis
- **visualization-specialist**: Data visualization creation
- **code-generator**: Analysis code generation
- **report-writer**: Comprehensive report generation
- **quality-assurance**: Data quality validation
- **hypothesis-generator**: Research hypothesis generation

### Slash Commands
- `/analyze [dataset] [analysis_type]`: Perform data analysis
- `/visualize [dataset] [chart_type]`: Create visualizations
- `/generate [language] [analysis_type]`: Generate analysis code
- `/report [dataset] [format]`: Generate analysis reports
- `/quality [dataset] [action]`: Perform data quality checks
- `/hypothesis [dataset] [domain]`: Generate research hypotheses

### Directory Structure
```
claude-data-analysis/
├── .claude/
│   ├── agents/          # Sub-agent configurations
│   ├── commands/        # Slash command definitions
│   ├── hooks/          # Automation scripts
│   └── settings.json   # Claude Code settings
├── data_storage/       # Data files directory
├── visualizations/     # Generated charts and plots
├── examples/          # Example datasets and workflows
└── docs/             # Documentation
```

## Usage Example

```bash
# Analyze user behavior data
/analyze user_behavior.csv exploratory

# Create visualizations
/visualize user_behavior.csv user-journey

# Generate analysis code
/generate python user-segmentation

# Create comprehensive report
/report user_behavior.csv complete html
```

## Configuration

The project uses Claude Code's configuration system:
- Sub-agents are defined in `.claude/agents/`
- Commands are stored in `.claude/commands/`
- Hooks are configured in `.claude/settings.json`

## Key Workflows

1. **Data Exploration**: Upload data → Run exploratory analysis → Review insights
2. **Visualization**: Analyze data → Generate visualizations → Export charts
3. **Reporting**: Complete analysis → Generate report → Share findings
4. **Code Generation**: Define requirements → Generate code → Test implementation

## Integration Notes

- Works with common data formats (CSV, JSON, Excel, SQL)
- Integrates with Python data science ecosystem
- Supports multiple visualization libraries
- Provides hooks for automation and quality control


## 注意要点

- 详细的分析代码和相关文档需要保存在项目中，可以进一步方便查看具体的分析过程和数据验证结果。
- 报告和文档请尽量用中文
- visualization画图注意中文字体问题！
