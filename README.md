# AutoStructor
AutoStructor: A Generative AI-Based Framework for Automated Program Repair with Deep Learning-Guided Fault Localization

## 1. COMPLEXITY METRICS

| Metric Name | Description |
|-------------|-------------|
| Cyclomatic Complexity | Measures the number of decision points in code |
| Cognitive Complexity | Measures cognitive load for understanding code |
| Nesting Depth | Maximum nesting level of control structures |
| Method Length | Number of lines of code in method |
| Parameter Count | Number of method parameters |
| Return Complexity | Complexity of return statements |

## 2. DESIGN QUALITY METRICS

| Metric Name | Description |
|-------------|-------------|
| SRP Score | Single Responsibility Principle adherence |
| Afferent Coupling | Number of incoming dependencies |
| Efferent Coupling | Number of outgoing dependencies |
| Cohesion Score | Relationship between elements within method |
| Abstraction Level | Level of abstraction vs concrete implementation |
| Pattern Usage | Number of design patterns used |

## 3. CODE QUALITY METRICS

| Metric Name | Description |
|-------------|-------------|
| Naming Quality | Quality of variable and method names |
| Comment Ratio | Ratio of comments to code lines |
| Code Smells | Number of code smell instances |
| Duplication Score | Amount of code duplication |
| Magic Numbers | Number of magic numbers in code |

## 4. MAINTAINABILITY METRICS

| Metric Name | Description |
|-------------|-------------|
| Readability Score | Code readability assessment |
| Testability Score | How easily the code can be tested |
| Reusability Score | Code reusability potential |
| Error Handling | Quality of error handling implementation |

## Summary

- **Total Metrics**: 21 quality metrics
- **Processing**: All metrics are normalized
- **Integration**: Combined with dependency graph and code change information as features
- **Purpose**: Enhance fault localization accuracy in software systems
