# API 设计助手

> 专业的 RESTful API 设计提示词

## 功能说明

这是一个专业的 API 设计助手 Prompt，帮助团队设计高质量的 RESTful API，覆盖接口设计、请求响应规范、错误处理、版本管理等维度。

## 适用场景

- 新 API 设计
- API 重构优化
- API 规范制定
- 接口评审准备
- OpenAPI 文档生成

## API 设计原则

| 原则 | 说明 |
|------|------|
| 资源导向 | 使用名词而非动词 |
| 层级结构 | 使用 URI 路径表达层级 |
| HTTP 语义 | 正确使用 HTTP 方法和状态码 |
| 统一格式 | 请求响应格式一致 |

## 命名规范

### URI 规范

| 规范 | 示例 |
|------|------|
| 使用小写 | `/users` |
| 用 `-` 分隔 | `/user-profiles` |
| 用复数名词 | `/users` |
| 嵌套表示层级 | `/users/{id}/orders` |

### HTTP 方法对应

| 方法 | 用途 | 示例 |
|------|------|------|
| GET | 获取资源 | GET /users |
| POST | 创建资源 | POST /users |
| PUT | 完整更新 | PUT /users/{id} |
| PATCH | 部分更新 | PATCH /users/{id} |
| DELETE | 删除资源 | DELETE /users/{id} |

## 使用方式

### 基本用法

```markdown
请为以下功能设计 API：

【功能描述】
[描述需要设计的 API 功能]

【业务场景】
[描述业务场景]

【资源实体】
[列出相关的数据实体]
```

### 详细模式

```markdown
请设计详细的 API 方案：

【功能描述】
[描述功能]

【数据实体】
[实体定义]

【约束要求】
[如：必须兼容现有 API、版本要求等]
```

## 输出模板

```markdown
## API 设计文档

### 接口列表

| 方法 | 路径 | 描述 |
|------|------|------|
| GET | /users | 获取用户列表 |

### 接口详情

**GET /users/{id}**

请求参数：
| 参数 | 位置 | 类型 | 必填 | 说明 |
|------|------|------|------|------|
| id | path | string | 是 | 用户ID |

响应示例：
```json
{
  "code": 0,
  "data": {}
}
```
```

## 相关文件

- [api-design-guide_prompt.md](./api-design-guide_prompt.md) - Prompt 原始文件
