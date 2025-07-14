

- Create ML Components
- LinearTimeSeriesForecaster
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this updatable estimator with a transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some UpdatableSupervisedEstimator, Self.Annotation> where Other : Transformer, Other.Input == Self.Transformer.Output
```

