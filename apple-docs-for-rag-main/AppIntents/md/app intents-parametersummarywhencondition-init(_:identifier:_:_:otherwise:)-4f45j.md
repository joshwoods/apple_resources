

- App Intents
- ParameterSummaryWhenCondition
-  init(\_:identifier:\_:\_:otherwise:) 

Initializer

# init(\_:identifier:\_:\_:otherwise:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ keyPath: KeyPath,
    identifier comparisonOperator: ComparableComparisonOperator,
    _ value: Parameter.Value.ValueType.ID,
    @ParameterSummaryBuilder _ when: () -> WhenCondition,
    @ParameterSummaryBuilder otherwise: () -> Otherwise
) where IntentType : AppIntent, Parameter : AnyIntentValue, Parameter.Value.ValueType : AppEntity, Parameter.Value.ValueType.ID == Int
```

