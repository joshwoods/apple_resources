

- Create ML Components
- TimeSeriesClassifier
- TimeSeriesClassifier.Model
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this temporal transformer with another temporal transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> ComposedTemporalTransformer where Other : TemporalTransformer, Self.Output == Other.Input
```

