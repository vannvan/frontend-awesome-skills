---
name: generate-api-service
description: |
  生成接口请求函数、封装service层代码
  关键词：接口、api、service、请求封装
---
# 技能：生成API Service请求函数
## 执行规则
1. 完整定义请求参数类型、返回数据类型
2. 使用项目默认请求库(默认假设使用axios，如果项目是别的库让用户补充)
3. 区分分页、普通查询、提交表单
4. 不硬编码baseURL

## 输出
service函数代码 + TS类型 + 调用示例
