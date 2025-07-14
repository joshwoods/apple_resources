

- Create ML Components
- LinearRegressor
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this supervised estimator with a temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
@preconcurrency
func appending(_ other: Other) -> some SupervisedTemporalEstimator, Other.Transformer>, Self.Annotation> where Other : TemporalEstimator, Self.Annotation : Sendable, Self.Transformer.Output == Other.Transformer.Input
```

