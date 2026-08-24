---
applyTo: "src/**/*.{ts,tsx}"
---
# 项目 AI 全局编码规范
## 技术栈
React19 + TypeScript + Vite
- 全部使用函数组件 + Hooks，禁止 class 组件
- ref 使用 React19 新语法：ref 作为普通 props 传入，优先不使用 forwardRef
- 表单异步优先使用 Action API、useActionState、useOptimistic、useFormStatus
- 允许使用 `use()` hook 在渲染阶段读取 Promise / Context，可以条件读取 Context
- 并发能力可使用 startTransition，优先不滥用 useMemo / useCallback；如果项目开启 React‑Compiler 则尽量移除手动缓存

## TS 类型约束
- 禁止 any，优先 type / interface 定义类型
- Props 类型显式声明，如果组件接收 ref，则 props 增加 `ref?: Ref<XXX>`
- 接口返回值必须定义类型

## 代码风格
- ESLint + Prettier
- 组件 PascalCase；自定义 Hooks useXxx 小驼峰
- 优先具名导出；默认导出仅入口文件
- UI组件和业务逻辑尽量拆分
- 复杂逻辑抽离函数 / 自定义hook
- 必要单行注释，拒绝过度冗余注释

## AI行为规则
1. 修改代码前，先读取当前已有文件，对齐现有项目写法
2. 信息不足时先提问，不要自行脑补业务字段
3. 不要生成已经废弃API：ReactDOM.render、旧版useFormState
4. 改动现有代码尽量给出变更要点
5. 生成组件时拆分：类型定义、组件主体、导出
