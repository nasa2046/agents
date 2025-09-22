# TDD 代理使用示例

本文档演示如何在 Claude Code 中使用与 TDD 相关的代理进行测试驱动开发工作流。

## TDD 编排代理

`tdd-orchestrator` 代理管理完整的 TDD 工作流，协调多个专业代理之间的工作。

### 基本用法

```bash
# 为新功能调用 TDD 编排器
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："使用 TDD 方法和 JWT 令牌实现用户身份验证"

# 编排器将：
# 1. 分析需求并设计测试策略
# 2. 与 test-automator 协调创建测试
# 3. 管理红-绿-重构循环
# 4. 跟踪指标并确保 TDD 合规性
```

### 高级编排

```bash
# 多团队 TDD 协调
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："协调前端、后端和移动团队购物车功能的 TDD 工作流"

# 基于属性的 TDD
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："使用基于属性的 TDD 和不变量检查实现排序算法"

# 遗留代码 TDD
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："在重构之前为遗留的 PaymentProcessor 类添加测试，使用特征测试"
```

## 具有 TDD 功能的测试自动化器

增强的 `test-automator` 代理现在包含全面的 TDD 支持。

### 测试优先开发

```bash
# 首先生成失败的测试
使用 Task 工具，设置 subagent_type="test-automator"
提示："为带有电子邮件验证的用户注册生成全面的失败测试。确保测试因正确原因而失败。"

# 增量测试开发
使用 Task 工具，设置 subagent_type="test-automator"
提示："为购物车创建增量测试套件：从添加项目开始，然后删除，然后计算总计"

# 基于属性的 TDD 测试
使用 Task 工具，设置 subagent_type="test-automator"
提示："使用 hypothesis/fast-check 为字符串工具库生成基于属性的测试"
```

### TDD 指标和合规性

```bash
# 跟踪 TDD 指标
使用 Task 工具，设置 subagent_type="test-automator"
提示："分析代码库并生成 TDD 合规性报告：测试优先百分比、周期时间、重构频率"

# 验证 TDD 纪律
使用 Task 工具，设置 subagent_type="test-automator"
提示："检查最近的提交是否遵循了 TDD：在实现之前编写测试"
```

## 特定语言的 TDD 示例

### Python TDD

```bash
使用 Task 工具，设置 subagent_type="python-pro"
提示："使用 pytest 和 TDD 方法实现二叉搜索树。从插入、搜索、删除操作的失败测试开始。"

使用 Task 工具，设置 subagent_type="test-automator"
提示："为 REST API 生成 Python pytest 测试，使用 TDD：首先编写契约测试，然后是单元测试，遵循芝加哥学派 TDD"
```

### JavaScript/TypeScript TDD

```bash
使用 Task 工具，设置 subagent_type="typescript-pro"
提示："使用 Jest 和 React Testing Library 通过 TDD 构建 React 组件。从行为测试开始，然后最小化实现。"

使用 Task 工具，设置 subagent_type="javascript-pro"
提示："使用 TDD 方法和 Mocha、Chai 实现 Express 中间件。使用模拟的伦敦学派。"
```

### Java TDD

```bash
使用 Task 工具，设置 subagent_type="java-pro"
提示："使用 JUnit 5 和 Mockito 通过 TDD 创建 Spring Boot 服务。从集成测试开始，然后是单元测试。"
```

### Go TDD

```bash
使用 Task 工具，设置 subagent_type="golang-pro"
提示："使用 Go 的测试包和 testify 通过 TDD 方法构建 gRPC 服务。包括表驱动测试。"
```

## TDD 工作流模式

### 经典红-绿-重构

```bash
# 第1步：RED - 编写失败测试
使用 Task 工具，设置 subagent_type="test-automator"
提示："为处理负数的斐波那契函数编写失败测试"

# 第2步：GREEN - 最小实现
使用 Task 工具，设置 subagent_type="python-pro"
提示："实现最小斐波那契函数以使测试通过"

# 第3步：REFACTOR - 改进代码
使用 Task 工具，设置 subagent_type="code-reviewer"
提示："重构斐波那契实现以提高性能，同时保持测试绿色"
```

### 由外而内 TDD（伦敦学派）

```bash
# 从验收测试开始
使用 Task 工具，设置 subagent_type="test-automator"
提示："使用 Cucumber/Gherkin 编写用户登录流程的验收测试"

# 使用模拟向内工作
使用 Task 工具，设置 subagent_type="test-automator"
提示："为带有模拟依赖项的登录控制器编写单元测试"

# 使用 TDD 实现
使用 Task 工具，设置 subagent_type="backend-architect"
提示："实现登录控制器以满足测试，使用依赖注入"
```

### 由内而外 TDD（芝加哥学派）

```bash
# 从单元测试开始
使用 Task 工具，设置 subagent_type="test-automator"
提示："为单个计算函数编写单元测试"

# 构建到集成
使用 Task 工具，设置 subagent_type="test-automator"
提示："编写组合计算函数的集成测试"

# 最终验收测试
使用 Task 工具，设置 subagent_type="test-automator"
提示："为完整计算工作流编写端到端测试"
```

## 专门的 TDD 场景

### 使用 TDD 进行 API 开发

```bash
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："
使用 TDD 为博客平台开发 REST API：
1. 从 OpenAPI 规范开始
2. 从规范生成契约测试
3. 测试优先实现端点
4. 添加集成测试
5. 包括性能测试
"
```

### 微服务 TDD

```bash
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："
使用 TDD 方法构建微服务：
- API 的契约测试
- 业务逻辑的单元测试
- 数据库的集成测试
- 服务的组件测试
- 工作流的端到端测试
"
```

### 前端组件 TDD

```bash
使用 Task 工具，设置 subagent_type="frontend-developer"
提示："
使用 TDD 构建日期选择器组件：
1. 测试组件渲染
2. 测试日期选择
3. 测试键盘导航
4. 测试可访问性
5. 测试日期验证
所有测试优先，然后实现
"
```

### 数据库迁移 TDD

```bash
使用 Task 工具，设置 subagent_type="database-optimizer"
提示："
使用 TDD 执行数据库迁移：
1. 为当前模式行为编写测试
2. 为所需模式行为编写测试
3. 实现迁移以通过两者
4. 包括回滚测试
"
```

## TDD 反模式检测

```bash
# 检测开发后测试
使用 Task 工具，设置 subagent_type="code-reviewer"
提示："审查最近的提交并识别在实现之后编写测试的地方"

# 查找过度模拟的测试
使用 Task 工具，设置 subagent_type="test-automator"
提示："分析测试套件并识别具有过度模拟但不测试真实行为的测试"

# 识别缺失的测试覆盖
使用 Task 工具，设置 subagent_type="test-automator"
提示："查找没有测试的代码路径，并建议遵循 TDD 方法的测试用例"
```

## TDD 指标和报告

```bash
# 生成 TDD 仪表板
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："创建 TDD 指标仪表板，显示：周期时间、测试优先百分比、重构频率、覆盖趋势"

# 团队 TDD 评估
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："评估团队的 TDD 成熟度水平并提供改进建议"

# TDD ROI 分析
使用 Task 工具，设置 subagent_type="business-analyst"
提示："计算 TDD 采用的 ROI：错误减少、开发速度、维护成本"
```

## TDD 学习和练习

```bash
# TDD 练习实践
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："使用严格的 TDD 指导我完成罗马数字练习"

# TDD 研讨会材料
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："创建带有团队培训练习的 TDD 研讨会"

# TDD 代码审查
使用 Task 工具，设置 subagent_type="code-reviewer"
提示："审查此代码的 TDD 最佳实践并提供具体的改进建议"
```

## 与 CI/CD 集成

```bash
# TDD 管道设置
使用 Task 工具，设置 subagent_type="deployment-engineer"
提示："设置强制执行 TDD 的 CI/CD 管道：验证在代码之前编写的测试，检查覆盖范围，跟踪指标"

# 提交前 TDD 钩子
使用 Task 工具，设置 subagent_type="dx-optimizer"
提示："创建确保在允许提交之前 TDD 合规性的 git 钩子"
```

## 不同架构的 TDD

### 使用 TDD 的六边形架构

```bash
使用 Task 工具，设置 subagent_type="architect-review"
提示："使用 TDD 实现六边形架构服务：从域测试开始，然后是端口，然后是适配器"
```

### 事件驱动 TDD

```bash
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："使用 TDD 构建事件驱动系统：测试事件生产、消费和编排"
```

### 无服务器 TDD

```bash
使用 Task 工具，设置 subagent_type="cloud-architect"
提示："使用 TDD 方法开发 Lambda 函数，包括本地测试和集成测试"
```

## 常见 TDD 命令组合

### 完整 TDD 功能开发

```bash
# 1. 使用编排器设计测试
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："为支付处理功能设计全面的测试策略"

# 2. 使用自动化器生成测试
使用 Task 工具，设置 subagent_type="test-automator"
提示："生成策略中识别的所有测试用例"

# 3. 使用语言专家实现
使用 Task 工具，设置 subagent_type="python-pro"
提示："增量实现支付处理以通过测试"

# 4. 审查和重构
使用 Task 工具，设置 subagent_type="code-reviewer"
提示："审查实现并建议重构，同时保持绿色测试"

# 5. 优化性能
使用 Task 工具，设置 subagent_type="performance-engineer"
提示："使用 TDD 方法优化支付处理性能"
```

### TDD 错误修复工作流

```bash
# 1. 使用测试重现
使用 Task 工具，设置 subagent_type="test-automator"
提示："编写重现错误 #123 的测试：用户无法使用特殊字符登录"

# 2. 最小修复
使用 Task 工具，设置 subagent_type="debugger"
提示："以最小更改修复错误以使测试通过"

# 3. 添加边缘情况
使用 Task 工具，设置 subagent_type="test-automator"
提示："为与错误相关的边缘情况添加其他测试用例"

# 4. 如需要则重构
使用 Task 工具，设置 subagent_type="code-reviewer"
提示："建议重构以防止类似错误"
```

## 代理使用的最佳实践

1. **从 tdd-orchestrator 开始** 用于需要协调的复杂功能
2. **使用 test-automator** 进行测试生成和验证
3. **利用特定语言代理** 用于实现阶段
4. **使用 code-reviewer** 用于重构阶段
5. **使用 business-analyst 跟踪** 用于指标和 ROI

## 故障排除

### 当测试不失败时

```bash
使用 Task 工具，设置 subagent_type="test-automator"
提示："验证当实现被移除时这些测试实际上会失败（变异测试）"
```

### 当 TDD 感觉缓慢时

```bash
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："优化 TDD 工作流以获得更快的反馈循环"
```

### 当团队抵制 TDD 时

```bash
使用 Task 工具，设置 subagent_type="tdd-orchestrator"
提示："为团队创建带有培训材料的渐进式 TDD 采用计划"
```

## 高级 TDD 技术

### 批准测试

```bash
使用 Task 工具，设置 subagent_type="test-automator"
提示："为复杂输出验证设置批准测试"
```

### 快照测试

```bash
使用 Task 工具，设置 subagent_type="test-automator"
提示："使用 TDD 为 UI 组件实现快照测试"
```

### 契约测试

```bash
使用 Task 工具，设置 subagent_type="test-automator"
提示："使用 TDD 方法和 Pact 在服务之间创建契约测试"
```

## 下一步

1. 尝试 [TDD 工作流命令](/workflows:tdd-cycle)
2. 使用 tdd-orchestrator 练习 TDD 练习
3. 将 TDD 代理集成到您的开发工作流中
4. 使用 test-automator 跟踪 TDD 指标
5. 与您的团队分享 TDD 成功案例