

- App Intents
-  ParameterSummaryWhenCondition 

Structure

# ParameterSummaryWhenCondition

A type that represents a conditional statement in a parameter summary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ParameterSummaryWhenCondition where Intent : AppIntent, WhenCondition : ParameterSummary, Otherwise : ParameterSummary
```

## Topics

### Creating a conditional statement

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, HasValueComparisonOperator, () -> WhenCondition, otherwise: () -> Otherwise)

enum EquatableComparisonOperator

Operators that indicate the type of equality check for a conditional statement.

enum ComparableComparisonOperator

Operators that indicate the type of comparison check for a conditional statement.

enum HasValueComparisonOperator

Operators that indicate the type of value check for a conditional statement.

enum OneOfComparisonOperator

Operators that indicate the type of containment check for a conditional statement.

### Initializers

init&lt;ValueType, Parameter>(KeyPath&lt;Intent, Parameter>, EquatableComparisonOperator, ValueType, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;ValueType, Parameter>(KeyPath&lt;Intent, Parameter>, ComparableComparisonOperator, ValueType, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Value, Parameter>(KeyPath&lt;Intent, Parameter>, ComparableComparisonOperator, Value.ValueType, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;ValueType, Parameter>(KeyPath&lt;Intent, Parameter>, EquatableComparisonOperator, ValueType.ValueType, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;ValueType, Parameter>(KeyPath&lt;Intent, Parameter>, OneOfComparisonOperator, [ValueType.ValueType], () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, identifier: ComparableComparisonOperator, Parameter.Value.ValueType.ID, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, identifier: EquatableComparisonOperator, String, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, identifier: OneOfComparisonOperator, [Parameter.Value.ValueType.ID], () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;IntentType, Parameter>(KeyPath&lt;IntentType, Parameter>, identifier: ComparableComparisonOperator, Parameter.Value.ValueType.ID, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, identifier: StringComparisonOperator, String, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;IntentType, Parameter>(KeyPath&lt;IntentType, Parameter>, identifier: StringComparisonOperator, String, () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, identifier: OneOfComparisonOperator, [String], () -> WhenCondition, otherwise: () -> Otherwise)

init&lt;Parameter>(KeyPath&lt;Intent, Parameter>, identifier: EquatableComparisonOperator, Parameter.Value.ValueType.ID, () -> WhenCondition, otherwise: () -> Otherwise)

init(widgetFamily: OneOfComparisonOperator, [IntentWidgetFamily], () -> WhenCondition, otherwise: () -> Otherwise)

init(widgetFamily: EquatableComparisonOperator, IntentWidgetFamily, () -> WhenCondition, otherwise: () -> Otherwise)

## Relationships

### Conforms To

- ParameterSummary

## See Also

### Shortcuts support

protocol ParameterSummary

An interface for defining the visual representation of an app intent’s parameters.

struct IntentParameterSummary

A type that describes the user interface configuration of an app intent’s parameters.

struct ParameterSummaryString

A human-readable string that interpolates parameter key paths to provide user-configurable placeholders in the Shortcuts app.

struct ParameterSummarySwitchCondition

A type that represents a switch statement in a parameter summary.

struct ParameterSummaryCaseCondition

A type that represents an individual case of a switch statement in a parameter summary.

struct ParameterSummaryDefaultCaseCondition

A type that represents the default case of a switch statement in a parameter summary.

