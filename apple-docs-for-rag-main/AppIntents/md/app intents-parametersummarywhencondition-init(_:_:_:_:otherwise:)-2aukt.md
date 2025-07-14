

- App Intents
- ParameterSummaryWhenCondition
-  init(\_:\_:\_:\_:otherwise:) 

Initializer

# init(\_:\_:\_:\_:otherwise:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ keyPath: KeyPath,
    _ comparisonOperator: ComparableComparisonOperator,
    _ value: ValueType,
    @ParameterSummaryBuilder _ when: () -> WhenCondition,
    @ParameterSummaryBuilder otherwise: () -> Otherwise
) where ValueType : Comparable, ValueType == Parameter.Value, Parameter : AnyIntentValue
```

