

- App Intents
-  ParameterSummaryBuilder 

Enumeration

# ParameterSummaryBuilder

A result builder that allows you to declaratively describe a parameter summary.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum ParameterSummaryBuilder where Intent : AppIntent
```

## Mentioned in 

Adding parameters to an app intent

## Overview

For more information about using parameters and providing a parameter summary, see Provide an interactive parameter summary for your intent.

## Topics

### Type Methods

static func buildBlock&lt;Summary>(Summary) -> Summary

static func buildExpression&lt;Summary>(Summary) -> Summary

## See Also

### Summarizing the parameters

associatedtype SummaryContent : ParameterSummary

The type of parameter summary representing this intent.

**Required**

static var parameterSummary: Self.SummaryContent

Defines the summary of this intent in relation to how its parameters are populated.

**Required** Default implementation provided.

static var parameterSummary: some ParameterSummary

typealias Parameter

typealias Case

typealias DefaultCase

typealias Summary

typealias Switch

typealias When

