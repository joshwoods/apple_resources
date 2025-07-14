

- App Intents
-  IntentParameterSummary 

Structure

# IntentParameterSummary

A type that describes the user interface configuration of an app intent’s parameters.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentParameterSummary where Intent : AppIntent
```

## Topics

### Crearing a parameter summary

init()

init(() -> [PartialKeyPath&lt;Intent>])

init(ParameterSummaryString&lt;Intent>, table: String?)

init(ParameterSummaryString&lt;Intent>, table: String?, () -> [PartialKeyPath&lt;Intent>])

### Building the parameter key paths

enum ParameterKeyPathsBuilder

A result builder that declaratively builds the path to a parameter.

## Relationships

### Conforms To

- ParameterSummary

## See Also

### Shortcuts support

protocol ParameterSummary

An interface for defining the visual representation of an app intent’s parameters.

struct ParameterSummaryString

A human-readable string that interpolates parameter key paths to provide user-configurable placeholders in the Shortcuts app.

struct ParameterSummaryWhenCondition

A type that represents a conditional statement in a parameter summary.

struct ParameterSummarySwitchCondition

A type that represents a switch statement in a parameter summary.

struct ParameterSummaryCaseCondition

A type that represents an individual case of a switch statement in a parameter summary.

struct ParameterSummaryDefaultCaseCondition

A type that represents the default case of a switch statement in a parameter summary.

