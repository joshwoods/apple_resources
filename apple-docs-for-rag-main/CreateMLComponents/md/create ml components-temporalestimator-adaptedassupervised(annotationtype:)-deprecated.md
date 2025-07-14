

- Create ML Components
- TemporalEstimator
-  adaptedAsSupervised(annotationType:) Deprecated

Instance Method

# adaptedAsSupervised(annotationType:)

Exposes this temporal estimator as a supervised temporal estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func adaptedAsSupervised(annotationType: Annotation.Type = Annotation.self) -> TemporalEstimatorToSupervisedAdaptor where Annotation : Equatable, Annotation : Sendable
```

## See Also

### Adapting and fitting

func fitted&lt;InputSequence>(to: InputSequence) async throws -> Self.TransformerDeprecated

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

Deprecated

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

Deprecated

