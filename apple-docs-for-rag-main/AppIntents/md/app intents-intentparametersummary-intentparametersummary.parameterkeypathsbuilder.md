

- App Intents
- IntentParameterSummary
-  IntentParameterSummary.ParameterKeyPathsBuilder 

Enumeration

# IntentParameterSummary.ParameterKeyPathsBuilder

A result builder that declaratively builds the path to a parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum ParameterKeyPathsBuilder
```

## Topics

### Building the path

static func buildBlock(PartialKeyPath&lt;Intent>...) -> [PartialKeyPath&lt;Intent>]

static func buildExpression&lt;ValueType>(KeyPath&lt;Intent, IntentParameter&lt;ValueType>>) -> PartialKeyPath&lt;Intent>

