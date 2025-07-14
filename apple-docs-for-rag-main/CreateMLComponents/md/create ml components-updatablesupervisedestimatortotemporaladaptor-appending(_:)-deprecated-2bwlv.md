

- Create ML Components
- UpdatableSupervisedEstimatorToTemporalAdaptor
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this updatable supervised temporal estimator with an updatable supervised estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some UpdatableSupervisedTemporalEstimator>, Self.Annotation> where Other : UpdatableSupervisedEstimator, Self.Annotation == Other.Annotation, Self.Transformer.Output == Other.Transformer.Input
```

