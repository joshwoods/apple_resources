

- Create ML Components
- UpdatableTemporalEstimatorToSupervisedAdaptor
-  update(\_:with:eventHandler:) Deprecated

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout UpdatableTemporalEstimatorToSupervisedAdaptor.Transformer,
    with input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, FeatureSequence.Feature == Estimator.Transformer.Input
```

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## See Also

### Fitting and updating

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

func update&lt;InputSequence, Validation, FeatureSequence>(inout UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

