

- App Intents
- AppIntent
-  AppIntent.Switch 

Type Alias

# AppIntent.Switch

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Switch = ParameterSummarySwitchCondition where Value : _IntentValue, CaseCondition : _ParameterSummarySwitchCase
```

## Mentioned in 

Adding parameters to an app intent

## See Also

### Summarizing the parameters

associatedtype SummaryContent : ParameterSummary

The type of parameter summary representing this intent.

**Required**

static var parameterSummary: Self.SummaryContent

Defines the summary of this intent in relation to how its parameters are populated.

**Required** Default implementation provided.

static var parameterSummary: some ParameterSummary

enum ParameterSummaryBuilder

A result builder that allows you to declaratively describe a parameter summary.

typealias Parameter

typealias Case

typealias DefaultCase

typealias Summary

typealias When

