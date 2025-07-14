

- Create ML Components
- UpdatableEstimatorToSupervisedAdaptor
-  update(\_:with:validateOn:eventHandler:) 

Instance Method

# update(\_:with:validateOn:eventHandler:)

Fits a transformer to a sequence of examples while validating with a validation sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout Estimator.Transformer,
    with input: InputSequence,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, Validation : Sequence, InputSequence.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature
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

### Fitting and Updating

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples, ignoring the annotations and the validation.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Estimator.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

typealias Transformer

The transformer type created by this estimator.

