---
name: create-hook
description: |
  用户需要创建自定义hook、封装状态逻辑、封装请求逻辑时触发
  关键词：自定义hook、封装hook、写一个useXXX
---
# 技能：创建自定义Hook
## 执行规则
1. Hook必须以 use 开头，小驼峰
2. 补齐完整TS入参、返回值类型，禁止any
3. 正确维护 useEffect 依赖数组
4. 如果是异步逻辑，优先给出两种可选方案：use + Suspense / useEffect
5. 副作用清理函数需要补充（定时器、事件监听等）
6. 不要在hook内硬编码业务常量

## 输出
完整hook代码 + 使用示例 + 参数说明
