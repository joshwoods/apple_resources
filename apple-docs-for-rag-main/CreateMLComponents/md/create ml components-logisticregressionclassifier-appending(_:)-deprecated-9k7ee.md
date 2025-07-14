

- Create ML Components
- LogisticRegressionClassifier
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this supervised estimator with a temporal transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
@preconcurrency
func appending(_ other: Other) -> some SupervisedTemporalEstimator, Other>, Self.Annotation> where Other : TemporalTransformer, Self.Annotation : Sendable, Other.Input == Self.Transformer.Output
```

