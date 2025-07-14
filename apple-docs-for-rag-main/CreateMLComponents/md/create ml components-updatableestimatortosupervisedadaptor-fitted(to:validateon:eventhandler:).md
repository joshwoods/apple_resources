

- Create ML Components
- UpdatableEstimatorToSupervisedAdaptor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a transformer to a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> UpdatableEstimatorToSupervisedAdaptor.Transformer where Input : Sequence, Validation : Sequence, Input.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`validation`  

A sequence of examples used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting and Updating

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples, ignoring the annotations and the validation.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update&lt;InputSequence>(inout Estimator.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

func update&lt;InputSequence, Validation>(inout Estimator.Transformer, with: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws

Fits a transformer to a sequence of examples while validating with a validation sequence.

typealias Transformer

The transformer type created by this estimator.

