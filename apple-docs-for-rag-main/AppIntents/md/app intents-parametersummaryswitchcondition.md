

- App Intents
-  ParameterSummarySwitchCondition 

Structure

# ParameterSummarySwitchCondition

A type that represents a switch statement in a parameter summary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ParameterSummarySwitchCondition where Intent : AppIntent, Value : _IntentValue, CaseCondition : _ParameterSummarySwitchCase
```

## Topics

### Creating a switch condition

enum ParameterSummaryCaseBuilder

A result builder that allows you to declaratively describe the cases of a switch statement in a parameter summary.

### Initializers

init(ParameterSummarySwitchCondition&lt;Intent, Value, CaseCondition>.WidgetFamily, () -> CaseCondition)

Initializes a parameter summary Switch statement over widget family.

init(KeyPath&lt;Intent, IntentParameter&lt;Value>>, () -> CaseCondition)

### Enumerations

enum WidgetFamily

An enum that represents a parameter summary Switch statement over widget family.

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

struct ParameterSummaryWhenCondition

A type that represents a conditional statement in a parameter summary.

struct ParameterSummaryCaseCondition

A type that represents an individual case of a switch statement in a parameter summary.

struct ParameterSummaryDefaultCaseCondition

A type that represents the default case of a switch statement in a parameter summary.

