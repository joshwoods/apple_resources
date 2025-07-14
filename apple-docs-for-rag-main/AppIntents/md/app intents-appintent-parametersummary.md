

- App Intents
- AppIntent
-  parameterSummary 

Type Property

# parameterSummary

Defines the summary of this intent in relation to how its parameters are populated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var parameterSummary: Self.SummaryContent { get }
```

**Required** Default implementation provided.

## Mentioned in 

Adding parameters to an app intent

## Discussion

For more information about using parameters and providing a parameter summary, see Provide an interactive parameter summary for your intent.

## Default Implementations

### AppIntent Implementations

static var parameterSummary: some ParameterSummary

## See Also

### Summarizing the parameters

associatedtype SummaryContent : ParameterSummary

The type of parameter summary representing this intent.

**Required**

static var parameterSummary: some ParameterSummary

enum ParameterSummaryBuilder

A result builder that allows you to declaratively describe a parameter summary.

typealias Parameter

typealias Case

typealias DefaultCase

typealias Summary

typealias Switch

typealias When

