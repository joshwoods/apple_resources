

- Create ML Components
- Estimator
-  adaptedAsTemporal() Deprecated

Instance Method

# adaptedAsTemporal()

Exposes this estimator as a temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func adaptedAsTemporal() -> EstimatorToTemporalAdaptor
```

## See Also

### Fitting and adapting

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> EstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this estimator as a supervised estimator.

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

func fitted&lt;S>(to: S) async throws -> Self.Transformer

