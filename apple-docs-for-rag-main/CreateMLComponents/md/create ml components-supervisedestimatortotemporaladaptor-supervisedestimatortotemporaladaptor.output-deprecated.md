

- Create ML Components
- SupervisedEstimatorToTemporalAdaptor
-  SupervisedEstimatorToTemporalAdaptor.Output Deprecated

Type Alias

# SupervisedEstimatorToTemporalAdaptor.Output

The output type.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
typealias Output = Base.Transformer.Output
```

## See Also

### Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

typealias Annotation

The annotation type.

Deprecated

typealias Input

The input type.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

