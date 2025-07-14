

- App Intents
-  ParameterSummaryDefaultCaseCondition 

Structure

# ParameterSummaryDefaultCaseCondition

A type that represents the default case of a switch statement in a parameter summary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ParameterSummaryDefaultCaseCondition where Intent : AppIntent, Value : _IntentValue, Summary : ParameterSummary
```

## Topics

### Creating the case condition

init(() -> Summary)

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

struct ParameterSummarySwitchCondition

A type that represents a switch statement in a parameter summary.

struct ParameterSummaryCaseCondition

A type that represents an individual case of a switch statement in a parameter summary.

