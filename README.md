# Common Prompt

研发常用 Prompt 集合，为开发团队提供高质量、可复用的 AI 提示词模板。

## 项目目标

收集和整理日常研发工作中常用的 AI 提示词，帮助团队：

- 提升代码质量和开发效率
- 规范文档生成和代码风格
- 加速技术方案设计和评审

## 目录结构

```
commonPrompt/
├── prompts/                      # Prompt 集合
│   ├── api-design/               # API 设计类
│   │   ├── api-design-guide.md
│   │   └── api-design-guide_prompt.md
│   ├── code-review/              # 代码审查类
│   │   ├── code-review-guide.md
│   │   └── code-review-guide_prompt.md
│   ├── code-refactor/           # 代码重构类
│   │   ├── code-refactor-guide.md
│   │   └── code-refactor-guide_prompt.md
│   ├── docs-generation/         # 文档生成类
│   │   ├── project-docs-generator.md
│   │   └── project-docs-generator_prompt.md
│   ├── tech-design/            # 技术设计类
│   │   ├── tech-design-guide.md
│   │   └── tech-design-guide_prompt.md
│   ├── testing/                # 测试相关类
│   │   ├── unit-test-generator.md
│   │   └── unit-test-generator_prompt.md
│   └── skill-safety/           # SKILL 安全防护类
│       ├── skill-safety-guard.md
│       └── skill-safety-guard_prompt.md
│
└── README.md                     # 项目说明文档
```

## Prompt 分类

### API 设计 (api-design)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [api-design-guide](./prompts/api-design/api-design-guide.md) | RESTful API 设计指南 | 新 API 设计、API 重构、接口评审 |

### 代码审查 (code-review)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [code-review-guide](./prompts/code-review/code-review-guide.md) | 通用代码审查指南 | Pull Request 审查、代码质量评估 |

### 代码重构 (code-refactor)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [code-refactor-guide](./prompts/code-refactor/code-refactor-guide.md) | 代码重构建议与实施 | 遗留代码优化、技术债务清理 |

### 文档生成 (docs-generation)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [project-docs-generator](./prompts/docs-generation/project-docs-generator.md) | AI 软件工程项目学习文档生成 | 新项目文档初始化、现有项目文档补充 |

### 技术设计 (tech-design)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [tech-design-guide](./prompts/tech-design/tech-design-guide.md) | 技术方案设计指南 | 新项目技术方案、重构方案、技术选型评估 |

### 测试相关 (testing)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [unit-test-generator](./prompts/testing/unit-test-generator.md) | 单元测试用例生成 | 补齐测试覆盖、测试驱动开发 |

### SKILL 安全防护 (skill-safety)

| Prompt 名称 | 功能说明 | 适用场景 |
|------------|----------|----------|
| [skill-safety-guard](./prompts/skill-safety/skill-safety-guard.md) | SKILL 调用安全防护规则 | 规范 AI Agent 高风险操作行为 |

## 快速导航

| 你想做什么？ | 使用哪个 Prompt？ |
|------------|------------------|
| 为新项目生成文档 | [project-docs-generator](./prompts/docs-generation/project-docs-generator.md) |
| 审查代码质量 | [code-review-guide](./prompts/code-review/code-review-guide.md) |
| 重构遗留代码 | [code-refactor-guide](./prompts/code-refactor/code-refactor-guide.md) |
| 设计 API 接口 | [api-design-guide](./prompts/api-design/api-design-guide.md) |
| 设计技术方案 | [tech-design-guide](./prompts/tech-design/tech-design-guide.md) |
| 生成单元测试 | [unit-test-generator](./prompts/testing/unit-test-generator.md) |
| 规范高风险操作 | [skill-safety-guard](./prompts/skill-safety/skill-safety-guard.md) |

## 使用规范

### 文件命名规则

每个 Prompt 包含两个文件：

| 文件类型 | 命名规则 | 说明 |
|----------|----------|------|
| 功能说明文件 | `{name}.md` | 包含功能描述、使用说明、适用场景 |
| Prompt 原始文件 | `{name}_prompt.md` | 完整的 AI 提示词内容 |

**命名规范：**

- 目录名使用小写，多词用 `-` 分割
- 文件名使用小写，多词用 `-` 分割
- 禁止使用下划线开头

## 快速开始

### 方式一：直接复制

1. 找到需要的 Prompt 功能说明文件
2. 阅读使用说明和适用场景
3. 复制对应的 `_prompt.md` 文件内容
4. 在 AI 对话中粘贴使用

### 方式二：项目引用

将 Prompt 文件作为上下文引用，让 AI 理解项目规范：

```markdown
请参考以下 Prompt 来完成代码审查任务：
{paste prompt content here}
```

## 贡献指南

欢迎提交新的 Prompt 或改进现有内容。

### 提交新 Prompt

1. 在 `prompts/` 下创建分类目录（如 `new-category/`）
2. 创建功能说明文件：`new-category/new-prompt.md`
3. 创建 Prompt 原始文件：`new-category/new-prompt_prompt.md`
4. 更新本 README 的分类表格

### Prompt 质量标准

- [ ] 提供清晰的功能说明和使用场景
- [ ] 包含实际可用的示例
- [ ] 避免歧义性描述
- [ ] 适配主流 AI 模型

## 更新日志

### v1.1.0 (2026-05-13)

- 新增 SKILL 安全防护 (skill-safety) 分类
- 添加 skill-safety-guard：规范 AI Agent 高风险操作行为

### v1.0.0 (2026-05-13)

- 初始化项目结构
- 添加以下 Prompt：
  - API 设计 (api-design)
  - 代码审查 (code-review)
  - 代码重构 (code-refactor)
  - 文档生成 (docs-generation)
  - 技术设计 (tech-design)
  - 测试相关 (testing)
- 定义文件命名规范

---

如有问题或建议，请提交 Issue 或 Pull Request。
