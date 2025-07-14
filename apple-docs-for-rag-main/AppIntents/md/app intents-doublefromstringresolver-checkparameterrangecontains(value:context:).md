

- App Intents
- DoubleFromStringResolver
-  checkParameterRangeContains(value:context:) 

Instance Method

# checkParameterRangeContains(value:context:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func checkParameterRangeContains(
    value: Value,
    context: IntentParameterContext
) throws where Value : RangeComparableProperty, Value == Self.Output.ValueType, Self.Output : Sendable
```

