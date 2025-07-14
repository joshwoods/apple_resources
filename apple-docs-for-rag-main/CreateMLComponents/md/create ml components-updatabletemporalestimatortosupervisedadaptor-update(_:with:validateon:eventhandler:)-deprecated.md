

- Create ML Components
- UpdatableTemporalEstimatorToSupervisedAdaptor
-  update(\_:with:validateOn:eventHandler:) Deprecated

Instance Method

# update(\_:with:validateOn:eventHandler:)

Fits a transformer to a sequence of examples while validating with a validation sequence.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func update(
    _ transformer: inout UpdatableTemporalEstimatorToSupervisedAdaptor.Transformer,
    with input: InputSequence,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, Validation : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature, FeatureSequence.Feature == Estimator.Transformer.Input
```

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`validation`  

A sequence of examples used for validation.

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

func update&lt;InputSequence, FeatureSequence>(inout UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

