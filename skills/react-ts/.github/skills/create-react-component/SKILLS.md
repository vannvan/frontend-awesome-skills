---
name: create-react-component
description: |
  用户需要新建React tsx组件、UI组件、业务组件、表单组件时触发
  关键词：新建组件、创建tsx、生成组件、写一个组件
---
# 技能：创建 React19 + TS 组件
## 执行规则
1. 使用React19语法，接收ref时直接在props解构，默认不使用forwardRef
2. 必须定义 Props 类型，不允许 any
3. 文件结构顺序：类型定义 → 组件 → 导出
4. 如果是表单组件，优先考虑 Action、useActionState
5. 样式如果没指定方案，只输出jsx逻辑，不强行引入UI库
6. 组件使用 PascalCase 命名，具名导出优先

## 输出格式
1. 完整可直接保存的tsx代码
2. 简短说明：Props参数、组件能力、注意事项
3. 如果组件支持ref，标明ref绑定目标DOM
