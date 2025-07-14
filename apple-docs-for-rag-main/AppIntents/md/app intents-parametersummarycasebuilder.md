

- App Intents
-  ParameterSummaryCaseBuilder 

Enumeration

# ParameterSummaryCaseBuilder

A result builder that allows you to declaratively describe the cases of a switch statement in a parameter summary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum ParameterSummaryCaseBuilder where Intent : AppIntent, Value : _IntentValue
```

## Topics

### Building switch statement cases

static func buildBlock&lt;C0, DefaultSummary>(C0, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, DefaultSummary>(C0, C1, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, DefaultSummary>(C0, C1, C2, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, DefaultSummary>(C0, C1, C2, C3, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, DefaultSummary>(C0, C1, C2, C3, C4, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, DefaultSummary>(C0, C1, C2, C3, C4, C5, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13, C14, DefaultSummary>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13, C14, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>) -> ParameterSummaryTupleCaseCondition&lt;Intent, Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13, C14, ParameterSummaryDefaultCaseCondition&lt;Intent, Value, DefaultSummary>)>

struct ParameterSummaryTupleCaseCondition

A type that represents a collection of case conditions for a specific switch statement.

### Type Methods

static func buildExpression&lt;C0>(C0) -> C0

