

- Create ML Components
- PreprocessingEstimator
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this estimator with a supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> some SupervisedTemporalEstimator, Other.Transformer>, Other.Annotation> where Other : SupervisedTemporalEstimator, Self.Transformer.Output == Other.Transformer.Input
```

