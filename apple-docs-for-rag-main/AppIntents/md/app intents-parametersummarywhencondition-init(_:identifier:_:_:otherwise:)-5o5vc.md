

- App Intents
- ParameterSummaryWhenCondition
-  init(\_:identifier:\_:\_:otherwise:) 

Initializer

# init(\_:identifier:\_:\_:otherwise:)

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
init(
    _ keyPath: KeyPath,
    identifier comparisonOperator: StringComparisonOperator,
    _ value: String,
    @ParameterSummaryBuilder _ when: () -> WhenCondition,
    @ParameterSummaryBuilder otherwise: () -> Otherwise
) where Parameter : AnyIntentValue, Parameter.Value.ValueType : AppEntity
```

