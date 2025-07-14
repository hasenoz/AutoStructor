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

## Implementation Details

### Normalization Thresholds
| Metric Category | Threshold Values |
|----------------|------------------|
| **Complexity Metrics** | Cyclomatic/Cognitive: (1,20), Nesting: (1,10), Method Length: (1,100), Parameters: (0,10), Return: (1,10) |
| **Coupling Metrics** | Afferent: (0,20), Efferent: (0,30) |
| **Quality Metrics** | Code Smells: (0,10), Magic Numbers: (0,10), Pattern Usage: (0,5) |

### Quality Score Calculation Rules
| Score Type | Calculation Method |
|------------|-------------------|
| **Reusability Score** | Generic implementation: +0.2, Interface usage: +0.2, Low coupling (≤5): +0.3, High cohesion (>0.7): +0.3 |
| **Error Handling** | Try-catch usage: +0.4, Input validation: +0.3, Specific exceptions: +0.3 |

## Summary
- **Total Metrics**: 21 quality metrics across 4 categories
- **Integration**: Combined with dependency graph and code change information as neural network features
- **Purpose**: Enhance fault localization accuracy by incorporating software quality characteristics
