# Claude Code 子代理集合

一个全面的83个专业AI子代理集合，用于[Claude Code](https://docs.anthropic.com/en/docs/claude-code)，提供软件开发、基础设施和业务运营领域的特定领域专业知识。

## 概述

此仓库提供生产就绪的子代理，扩展Claude Code的功能，具有专业知识。每个子代理包含：

- 当前行业最佳实践和标准（2024/2025）
- 生产就绪模式和企业架构
- 每个代理8-12个能力领域
- 现代技术栈和框架
- 基于任务复杂度的优化模型选择

## 代理类别

### 架构与系统设计

#### 核心架构

| 代理 | 模型 | 描述 |
|------|------|------|
| [backend-architect](backend-architect.md) | opus | RESTful API设计、微服务边界、数据库模式 |
| [frontend-developer](frontend-developer.md) | sonnet | React组件、响应式布局、客户端状态管理 |
| [graphql-architect](graphql-architect.md) | opus | GraphQL模式、解析器、联邦架构 |
| [architect-reviewer](architect-review.md) | opus | 架构一致性分析和模式验证 |
| [cloud-architect](cloud-architect.md) | opus | AWS/Azure/GCP基础设施设计和成本优化 |
| [hybrid-cloud-architect](hybrid-cloud-architect.md) | opus | 多云策略，跨越云和本地环境 |
| [kubernetes-architect](kubernetes-architect.md) | opus | 使用Kubernetes和GitOps的云原生基础设施 |

#### UI/UX 与移动

| 代理 | 模型 | 描述 |
|------|------|------|
| [ui-ux-designer](ui-ux-designer.md) | sonnet | 接口设计、线框图、设计系统 |
| [ui-visual-validator](ui-visual-validator.md) | sonnet | 视觉回归测试和UI验证 |
| [mobile-developer](mobile-developer.md) | sonnet | React Native和Flutter应用开发 |
| [ios-developer](ios-developer.md) | sonnet | 使用Swift/SwiftUI的原生iOS开发 |
| [flutter-expert](flutter-expert.md) | sonnet | 高级Flutter开发，带状态管理 |

### 编程语言

#### 系统与低级

| 代理 | 模型 | 描述 |
|------|------|------|
| [c-pro](c-pro.md) | sonnet | 系统编程，带内存管理和OS接口 |
| [cpp-pro](cpp-pro.md) | sonnet | 现代C++，带RAII、智能指针、STL算法 |
| [rust-pro](rust-pro.md) | sonnet | 内存安全的系统编程，带所有权模式 |
| [golang-pro](golang-pro.md) | sonnet | 使用goroutines和channels的并发编程 |

#### Web 与应用

| 代理 | 模型 | 描述 |
|------|------|------|
| [javascript-pro](javascript-pro.md) | sonnet | 现代JavaScript，带ES6+、异步模式、Node.js |
| [typescript-pro](typescript-pro.md) | sonnet | 高级TypeScript，带类型系统和泛型 |
| [python-pro](python-pro.md) | sonnet | Python开发，带高级功能和优化 |
| [ruby-pro](ruby-pro.md) | sonnet | Ruby，带元编程、Rails模式、gem开发 |
| [php-pro](php-pro.md) | sonnet | 现代PHP，带框架和性能优化 |

#### 企业与JVM

| 代理 | 模型 | 描述 |
|------|------|------|
| [java-pro](java-pro.md) | sonnet | 现代Java，带流、并发、JVM优化 |
| [scala-pro](scala-pro.md) | sonnet | 企业Scala，带函数式编程和分布式系统 |
| [csharp-pro](csharp-pro.md) | sonnet | C#开发，带.NET框架和模式 |

#### 专业平台

| 代理 | 模型 | 描述 |
|------|------|------|
| [elixir-pro](elixir-pro.md) | sonnet | Elixir，带OTP模式和Phoenix框架 |
| [unity-developer](unity-developer.md) | sonnet | Unity游戏开发和优化 |
| [minecraft-bukkit-pro](minecraft-bukkit-pro.md) | sonnet | Minecraft服务器插件开发 |
| [sql-pro](sql-pro.md) | sonnet | 复杂SQL查询和数据库优化 |

### 基础设施与运营

#### DevOps 与部署

| 代理 | 模型 | 描述 |
|------|------|------|
| [devops-troubleshooter](devops-troubleshooter.md) | sonnet | 生产调试、日志分析、部署故障排除 |
| [deployment-engineer](deployment-engineer.md) | sonnet | CI/CD管道、容器化、云部署 |
| [terraform-specialist](terraform-specialist.md) | opus | 使用Terraform模块和状态管理的代码即基础设施 |
| [dx-optimizer](dx-optimizer.md) | sonnet | 开发者体验优化和工具改进 |

#### 数据库管理

| 代理 | 模型 | 描述 |
|------|------|------|
| [database-optimizer](database-optimizer.md) | opus | 查询优化、索引设计、迁移策略 |
| [database-admin](database-admin.md) | sonnet | 数据库操作、备份、复制、监控 |

#### 事件响应与网络

| 代理 | 模型 | 描述 |
|------|------|------|
| [incident-responder](incident-responder.md) | opus | 生产事件管理和解决 |
| [network-engineer](network-engineer.md) | sonnet | 网络调试、负载均衡、流量分析 |

### 质量保证与安全

#### 代码质量与审查

| 代理 | 模型 | 描述 |
|------|------|------|
| [code-reviewer](code-reviewer.md) | opus | 带安全焦点和生产可靠性的代码审查 |
| [security-auditor](security-auditor.md) | opus | 漏洞评估和OWASP合规 |
| [backend-security-coder](backend-security-coder.md) | opus | 安全的后端编码实践、API安全实现 |
| [frontend-security-coder](frontend-security-coder.md) | opus | XSS预防、CSP实现、客户端安全 |
| [mobile-security-coder](mobile-security-coder.md) | opus | 移动安全模式、WebView安全、生物识别认证 |
| [architect-reviewer](architect-review.md) | opus | 架构一致性和模式验证 |

#### 测试与调试

| 代理 | 模型 | 描述 |
|------|------|------|
| [test-automator](test-automator.md) | sonnet | 全面测试套件创建（单元、集成、e2e） |
| [tdd-orchestrator](tdd-orchestrator.md) | sonnet | 测试驱动开发方法指导 |
| [debugger](debugger.md) | sonnet | 错误解决和测试失败分析 |
| [error-detective](error-detective.md) | sonnet | 日志分析和错误模式识别 |

#### 性能与可观察性

| 代理 | 模型 | 描述 |
|------|------|------|
| [performance-engineer](performance-engineer.md) | opus | 应用剖析和优化 |
| [observability-engineer](observability-engineer.md) | opus | 生产监控、分布式跟踪、SLI/SLO管理 |
| [search-specialist](search-specialist.md) | haiku | 高级Web研究和信息合成 |

### 数据与AI

#### 数据工程与分析

| 代理 | 模型 | 描述 |
|------|------|------|
| [data-scientist](data-scientist.md) | opus | 数据分析、SQL查询、BigQuery操作 |
| [data-engineer](data-engineer.md) | sonnet | ETL管道、数据仓库、流架构 |

#### 机器学习与AI

| 代理 | 模型 | 描述 |
|------|------|------|
| [ai-engineer](ai-engineer.md) | opus | LLM应用、RAG系统、提示管道 |
| [ml-engineer](ml-engineer.md) | opus | ML管道、模型服务、特征工程 |
| [mlops-engineer](mlops-engineer.md) | opus | ML基础设施、实验跟踪、模型注册表 |
| [prompt-engineer](prompt-engineer.md) | opus | LLM提示优化和工程 |

### 文档与技术写作

| 代理 | 模型 | 描述 |
|------|------|------|
| [docs-architect](docs-architect.md) | opus | 全面技术文档生成 |
| [api-documenter](api-documenter.md) | sonnet | OpenAPI/Swagger规范和开发者文档 |
| [reference-builder](reference-builder.md) | haiku | 技术参考和API文档 |
| [tutorial-engineer](tutorial-engineer.md) | sonnet | 逐步教程和教育内容 |
| [mermaid-expert](mermaid-expert.md) | sonnet | 图表创建（流程图、序列图、ERD） |

### 业务与运营

#### 业务分析与财务

| 代理 | 模型 | 描述 |
|------|------|------|
| [business-analyst](business-analyst.md) | sonnet | 指标分析、报告、KPI跟踪 |
| [quant-analyst](quant-analyst.md) | opus | 财务建模、交易策略、市场分析 |
| [risk-manager](risk-manager.md) | sonnet | 投资组合风险监控和管理 |

#### 营销与销售

| 代理 | 模型 | 描述 |
|------|------|------|
| [content-marketer](content-marketer.md) | sonnet | 博客文章、社交媒体、电子邮件活动 |
| [sales-automator](sales-automator.md) | haiku | 冷邮件、跟进、提案生成 |

#### 支持与法律

| 代理 | 模型 | 描述 |
|------|------|------|
| [customer-support](customer-support.md) | sonnet | 支持票据、FAQ响应、客户沟通 |
| [hr-pro](hr-pro.md) | opus | HR操作、政策、员工关系 |
| [legal-advisor](legal-advisor.md) | opus | 隐私政策、服务条款、法律文档 |

### 专业领域

| 代理 | 模型 | 描述 |
|------|------|------|
| [blockchain-developer](blockchain-developer.md) | sonnet | Web3应用、智能合约、DeFi协议 |
| [payment-integration](payment-integration.md) | sonnet | 支付处理器集成（Stripe、PayPal） |
| [legacy-modernizer](legacy-modernizer.md) | sonnet | 遗留代码重构和现代化 |
| [context-manager](context-manager.md) | haiku | 多代理上下文管理 |

### SEO 与内容优化

| 代理 | 模型 | 描述 |
|------|------|------|
| [seo-content-auditor](seo-content-auditor.md) | sonnet | 内容质量分析、E-E-A-T信号评估 |
| [seo-meta-optimizer](seo-meta-optimizer.md) | haiku | 元标题和描述优化 |
| [seo-keyword-strategist](seo-keyword-strategist.md) | haiku | 关键词分析和语义变体 |
| [seo-structure-architect](seo-structure-architect.md) | haiku | 内容结构和schema标记 |
| [seo-snippet-hunter](seo-snippet-hunter.md) | haiku | 特色片段格式化 |
| [seo-content-refresher](seo-content-refresher.md) | haiku | 内容新鲜度分析 |
| [seo-cannibalization-detector](seo-cannibalization-detector.md) | haiku | 关键词重叠检测 |
| [seo-authority-builder](seo-authority-builder.md) | sonnet | E-E-A-T信号分析 |
| [seo-content-writer](seo-content-writer.md) | sonnet | SEO优化内容创建 |
| [seo-content-planner](seo-content-planner.md) | haiku | 内容规划和主题集群 |

## 模型配置

代理根据任务复杂度和计算需求分配到特定Claude模型。系统使用三个模型层级：

### 模型分布摘要

| 模型 | 代理数量 | 用例 |
|------|----------|------|
| Haiku | 11 | 快速、专注任务，最小计算开销 |
| Sonnet | 46 | 标准开发和专业工程任务 |
| Opus | 22 | 复杂推理、架构和关键分析 |

### Haiku模型代理

| 类别 | 代理 |
|------|------|
| 上下文与参考 | `context-manager`、`reference-builder`、`sales-automator`、`search-specialist` |
| SEO优化 | `seo-meta-optimizer`、`seo-keyword-strategist`、`seo-structure-architect`、`seo-snippet-hunter`、`seo-content-refresher`、`seo-cannibalization-detector`、`seo-content-planner` |

### Sonnet模型代理

| 类别 | 数量 | 代理 |
|------|------|------|
| 编程语言 | 18 | 所有语言特定代理（JavaScript、Python、Java、C++等） |
| 前端与UI | 5 | `frontend-developer`、`ui-ux-designer`、`ui-visual-validator`、`mobile-developer`、`ios-developer` |
| 基础设施 | 8 | `devops-troubleshooter`、`deployment-engineer`、`dx-optimizer`、`database-admin`、`network-engineer`、`flutter-expert`、`api-documenter`、`tutorial-engineer` |
| 质量与测试 | 4 | `test-automator`、`tdd-orchestrator`、`debugger`、`error-detective` |
| 业务与支持 | 6 | `business-analyst`、`risk-manager`、`content-marketer`、`customer-support`、`mermaid-expert`、`legacy-modernizer` |
| 数据与内容 | 5 | `data-engineer`、`payment-integration`、`seo-content-auditor`、`seo-authority-builder`、`seo-content-writer` |

### Opus模型代理

| 类别 | 数量 | 代理 |
|------|------|------|
| 架构与设计 | 7 | `architect-reviewer`、`backend-architect`、`cloud-architect`、`hybrid-cloud-architect`、`kubernetes-architect`、`graphql-architect`、`terraform-specialist` |
| 关键分析 | 6 | `code-reviewer`、`security-auditor`、`performance-engineer`、`observability-engineer`、`incident-responder`、`database-optimizer` |
| AI/ML复杂 | 5 | `ai-engineer`、`ml-engineer`、`mlops-engineer`、`data-scientist`、`prompt-engineer` |
| 业务关键 | 4 | `docs-architect`、`hr-pro`、`legal-advisor`、`quant-analyst` |

## 安装

将仓库克隆到Claude代理目录：

```bash
cd ~/.claude
git clone https://github.com/wshobson/agents.git
```

子代理放置在`~/.claude/agents/`目录后，将自动可用给Claude Code。

## 使用

### 自动委托

Claude Code根据任务上下文和需求自动选择合适的子代理。系统分析您的请求并委托给最合适的专家。

### 显式调用

通过名称指定子代理以使用特定专家：

```
"使用code-reviewer分析最近更改"
"让security-auditor扫描漏洞"
"让performance-engineer优化此瓶颈"
```

## 使用示例

### 代码质量与安全
```
code-reviewer: 分析组件的最佳实践
security-auditor: 检查OWASP合规
tdd-orchestrator: 使用测试优先方法实现功能
performance-engineer: 剖析和优化瓶颈
```

### 开发与架构
```
backend-architect: 设计认证API
frontend-developer: 创建响应式仪表板
graphql-architect: 设计联邦GraphQL模式
mobile-developer: 构建跨平台移动应用
```

### 基础设施与运营
```
devops-troubleshooter: 分析生产日志
cloud-architect: 设计可扩展的AWS架构
network-engineer: 调试SSL证书问题
database-admin: 配置备份和复制
terraform-specialist: 编写基础设施模块
```

### 数据与机器学习
```
data-scientist: 分析客户行为数据集
ai-engineer: 为文档搜索构建RAG系统
mlops-engineer: 设置实验跟踪
ml-engineer: 将模型部署到生产
```

### 业务与文档
```
business-analyst: 创建指标仪表板
docs-architect: 生成技术文档
api-documenter: 编写OpenAPI规范
content-marketer: 创建SEO优化内容
```

## 多代理工作流

子代理自动协调复杂任务。系统根据任务需求智能序列多个专家。

### 常见工作流模式

**功能开发**
```
"实现用户认证"
→ backend-architect → frontend-developer → test-automator → security-auditor
```

**性能优化**
```
"优化结账过程"
→ performance-engineer → database-optimizer → frontend-developer
```

**生产事件**
```
"调试高内存使用"
→ incident-responder → devops-troubleshooter → error-detective → performance-engineer
```

**基础设施设置**
```
"设置灾难恢复"
→ database-admin → database-optimizer → terraform-specialist
```

**ML管道开发**
```
"构建带监控的ML管道"
→ mlops-engineer → ml-engineer → data-engineer → performance-engineer
```

### 与Claude Code命令集成

对于复杂的多代理编排，使用[Claude Code Commands](https://github.com/wshobson/commands)集合，提供52个预构建斜杠命令：

```
/full-stack-feature   # 协调8+代理完成功能开发
/incident-response    # 激活事件管理工作流
/ml-pipeline         # 设置端到端ML基础设施
/security-hardening  # 在栈中实现安全最佳实践
```

## 子代理格式

每个子代理定义为带frontmatter的Markdown文件：

```markdown
---
name: subagent-name
description: 此子代理的激活标准
model: haiku|sonnet|opus  # 可选：模型选择
tools: tool1, tool2       # 可选：工具限制
---

定义子代理专业知识和行为的系统提示
```

### 模型选择标准

- **haiku**：简单、确定性任务，最小推理
- **sonnet**：标准开发和工程任务
- **opus**：复杂分析、架构和关键操作

## 代理编排模式

### 顺序处理

代理顺序执行，向前传递上下文：
```
backend-architect → frontend-developer → test-automator → security-auditor
```

### 并行执行

多个代理同时处理不同方面：
```
performance-engineer + database-optimizer → 合并分析
```

### 条件路由

基于分析的动态代理选择：
```
debugger → [backend-architect | frontend-developer | devops-troubleshooter]
```

### 验证管道

主要工作后跟专业审查：
```
payment-integration → security-auditor → 验证实现
```

## 代理选择指南

### 架构与规划

| 任务 | 推荐代理 | 关键能力 |
|------|----------|----------|
| API设计 | `backend-architect` | RESTful API、微服务、数据库模式 |
| 云基础设施 | `cloud-architect` | AWS/Azure/GCP设计、可扩展性规划 |
| UI/UX设计 | `ui-ux-designer` | 接口设计、线框图、设计系统 |
| 系统架构 | `architect-reviewer` | 模式验证、一致性分析 |

### 按语言开发

| 语言类别 | 代理 | 主要用例 |
|----------|------|----------|
| 系统编程 | `c-pro`、`cpp-pro`、`rust-pro`、`golang-pro` | OS接口、嵌入式系统、高性能 |
| Web开发 | `javascript-pro`、`typescript-pro`、`python-pro`、`ruby-pro`、`php-pro` | 全栈Web应用、API、脚本 |
| 企业 | `java-pro`、`csharp-pro`、`scala-pro` | 大规模应用、企业系统 |
| 移动 | `ios-developer`、`flutter-expert`、`mobile-developer` | 原生和跨平台移动应用 |
| 专业 | `elixir-pro`、`unity-developer`、`minecraft-bukkit-pro` | 领域特定开发 |

### 运营与基础设施

| 任务 | 推荐代理 | 关键能力 |
|------|----------|----------|
| 生产问题 | `devops-troubleshooter` | 日志分析、部署调试 |
| 关键事件 | `incident-responder` | 宕机响应、即时缓解 |
| 数据库性能 | `database-optimizer` | 查询优化、索引策略 |
| 数据库操作 | `database-admin` | 备份、复制、灾难恢复 |
| 代码即基础设施 | `terraform-specialist` | Terraform模块、状态管理 |
| 网络问题 | `network-engineer` | 网络调试、负载均衡 |

### 质量与安全

| 任务 | 推荐代理 | 关键能力 |
|------|----------|----------|
| 代码审查 | `code-reviewer` | 安全焦点、最佳实践 |
| 安全审计 | `security-auditor` | 漏洞扫描、OWASP合规 |
| 测试创建 | `test-automator` | 单元、集成、E2E测试套件 |
| 性能问题 | `performance-engineer` | 剖析、优化 |
| 错误调查 | `debugger` | 错误解决、根本原因分析 |

### 数据与机器学习

| 任务 | 推荐代理 | 关键能力 |
|------|----------|----------|
| 数据分析 | `data-scientist` | SQL查询、统计分析 |
| LLM应用 | `ai-engineer` | RAG系统、提示管道 |
| ML开发 | `ml-engineer` | 模型训练、特征工程 |
| ML运营 | `mlops-engineer` | ML基础设施、实验跟踪 |

### 文档与业务

| 任务 | 推荐代理 | 关键能力 |
|------|----------|----------|
| 技术文档 | `docs-architect` | 全面文档生成 |
| API文档 | `api-documenter` | OpenAPI/Swagger规范 |
| 业务指标 | `business-analyst` | KPI跟踪、报告 |
| 法律合规 | `legal-advisor` | 隐私政策、服务条款 |

## 最佳实践

### 任务委托

1. **自动选择** - 让Claude Code分析上下文并选择最佳代理
2. **明确要求** - 指定约束、技术栈和质量标准
3. **信任专业化** - 每个代理针对其特定领域优化

### 多代理工作流

1. **高层请求** - 允许代理协调复杂多步任务
2. **上下文保留** - 确保代理有必要背景信息
3. **集成审查** - 验证不同代理输出如何协同工作

### 显式控制

1. **直接调用** - 指定代理当需要特定专业知识时
2. **战略组合** - 使用多个专家进行验证
3. **审查模式** - 请求特定审查工作流（例如，"security-auditor审查API设计"）

### 性能优化

1. **监控有效性** - 跟踪哪些代理最适合您的用例
2. **迭代细化** - 使用代理反馈改进要求
3. **复杂性匹配** - 将任务复杂性与代理能力对齐

## 贡献

添加新子代理：

1. 创建带适当frontmatter的新`.md`文件
2. 使用小写、连字符分隔命名约定
3. 在description中编写清晰激活标准
4. 定义带专业领域全面系统提示

## 故障排除

### 代理未激活

- 确保请求明确指示领域
- 指定任务类型和要求
- 如果自动选择失败，使用显式调用

### 意外代理选择

- 提供更多关于技术栈的上下文
- 在请求中包含特定要求
- 使用直接代理命名进行精确控制

### 冲突推荐

- 正常行为 - 专家有不同优先级
- 请求特定代理之间的协调
- 基于项目要求考虑权衡

### 缺失上下文

- 在请求中包含背景信息
- 引用先前工作或模式
- 提供项目特定约束

## 许可

MIT许可 - 详见[LICENSE](LICENSE)文件。

## 资源

- [Claude Code文档](https://docs.anthropic.com/en/docs/claude-code)
- [子代理文档](https://docs.anthropic.com/en/docs/claude-code/sub-agents)
- [Claude Code GitHub](https://github.com/anthropics/claude-code)
- [Claude Code命令](https://github.com/wshobson/commands)