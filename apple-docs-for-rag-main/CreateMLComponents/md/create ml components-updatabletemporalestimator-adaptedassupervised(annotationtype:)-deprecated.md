

- Create ML Components
- UpdatableTemporalEstimator
-  adaptedAsSupervised(annotationType:) Deprecated

Instance Method

# adaptedAsSupervised(annotationType:)

Exposes this temporal estimator as a supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func adaptedAsSupervised(annotationType: Annotation.Type = Annotation.self) -> UpdatableTemporalEstimatorToSupervisedAdaptor where Annotation : Equatable, Annotation : Sendable
```

