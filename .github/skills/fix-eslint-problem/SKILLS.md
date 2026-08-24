---
name: fix-eslint-problem
description: |
  修复ESLint报错、Hooks依赖警告、语法错误
  关键词：修复eslint、lint报错、修复hooks依赖
---
# 技能：修复 ESLint / Hooks 依赖问题
## 执行规则
1. 优先分析真实原因，不要无脑添加空依赖 []
2. useEffect 依赖缺失：优先抽离稳定函数，其次使用 useCallback
3. 不要粗暴加 // eslint‑disable
4. 修改完成后说明报错原因、修复思路

## 输出
修复后代码 + 问题原因说明
