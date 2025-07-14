

- App Intents
- ParameterSummaryWhenCondition
-  init(widgetFamily:\_:\_:otherwise:) 

Initializer

# init(widgetFamily:\_:\_:otherwise:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    widgetFamily comparisonOperator: EquatableComparisonOperator,
    _ value: IntentWidgetFamily,
    @ParameterSummaryBuilder _ when: () -> WhenCondition,
    @ParameterSummaryBuilder otherwise: () -> Otherwise
)
```

