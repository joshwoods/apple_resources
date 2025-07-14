

- Create ML Components
- UpdatableEstimatorToTemporalAdaptor
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this updatable temporal estimator with an updatable supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some UpdatableSupervisedTemporalEstimator, Other.Annotation> where Other : UpdatableSupervisedTemporalEstimator, Self.Transformer.Output == Other.Transformer.Input
```

