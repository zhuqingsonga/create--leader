# create-leader - 领导.skill 创建器

基于colleague-skill设计思路，增加核心差异化场景："我该怎么取代这个领导"

## 核心功能

### Track 1：领导力模拟
- "如果是这位领导，他会怎么决策？"
- "这位领导在这个场景下会说什么？"

### Track 2：向上管理辅助
- "我该怎么向这位领导汇报？"
- "这个方案怎么说服这位领导？"

### Track 3：取代路径规划（核心差异化）
- "我该怎么取代这个领导？"
- "这位领导的软肋是什么？"
- "我需要具备什么能力才能坐上这个位置？"

## 目录结构

```
leader-skill/
├── SKILL.md (主文件)
├── README.md (本文件)
└── prompts/
    ├── intake.md (基础信息录入)
    ├── leadership_analyzer.md (领导力模拟分析)
    ├── upward_analyzer.md (向上管理分析)
    └── replacement_analyzer.md (取代路径规划分析)
```

## 使用方式

1. `/create-leader` - 创建新的领导skill
2. `/list-leaders` - 列出所有已生成的领导
3. `/{slug}` - 使用完整的领导skill（包含三个模块）
4. `/{slug}-leadership` - 仅使用领导力模拟
5. `/{slug}-upward` - 仅使用向上管理
6. `/{slug}-replacement` - 仅使用取代路径规划

## 设计亮点

- **三轨结构**：Work（领导力）+ Upward（向上管理）+ Replacement（取代路径）
- **核心差异化**："取代路径规划"是这个skill的爆款功能
- **数据采集**：与colleague-skill类似，支持飞书/钉钉自动采集
- **持续进化**：支持追加文件 + 对话纠正 + 版本管理
- **伦理提醒**：明确提示仅用于个人成长参考

## 待完善

- `tools/` 目录下的Python脚本（数据采集、版本管理等）
- `prompts/` 目录下的其他文件（merger.md、correction_handler.md等）
- `assets/` 目录下的模板文件

## 灵感来源

基于 https://github.com/titanwings/colleague-skill 设计思路扩展
