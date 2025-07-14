

- Create ML Components
- TimeSeriesClassifier
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this updatable supervised estimator with an updatable temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
@preconcurrency
func appending(_ other: Other) -> some UpdatableSupervisedTemporalEstimator, Other.Transformer>, Self.Annotation> where Other : UpdatableTemporalEstimator, Self.Annotation : Sendable, Self.Transformer.Output == Other.Transformer.Input
```

