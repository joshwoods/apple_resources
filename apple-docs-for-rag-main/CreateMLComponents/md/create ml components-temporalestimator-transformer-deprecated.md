

- Create ML Components
- TemporalEstimator
-  Transformer Deprecated

Associated Type

# Transformer

The transformer type created by this estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
associatedtype Transformer : TemporalTransformer
```

**Required**

## See Also

### Adapting and fitting

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> TemporalEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this temporal estimator as a supervised temporal estimator.

Deprecated

func fitted&lt;InputSequence>(to: InputSequence) async throws -> Self.TransformerDeprecated

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

Deprecated

