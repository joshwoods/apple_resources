

- App Intents
-  RangeCheckingResolver 

Protocol

# RangeCheckingResolver

An interface for validating that a value is within a parameter’s defined inclusive range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol RangeCheckingResolver : Resolver
```

## Topics

### Checking the range of a parameter

func checkParameterRangeContains&lt;Value>(value: Value, context: IntentParameterContext&lt;Self.Output>) throws

## Relationships

### Inherits From

- Equatable
- Hashable
- Resolver
- Sendable

### Conforming Types

- DoubleFromIntResolver
- DoubleFromStringResolver
- DoubleResolver
- IntFromDoubleResolver
- IntFromStringResolver
- IntResolver

## See Also

### Range validation

protocol RangeComparableProperty

