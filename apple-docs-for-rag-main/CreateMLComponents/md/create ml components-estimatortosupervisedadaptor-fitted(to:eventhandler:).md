

- Create ML Components
- EstimatorToSupervisedAdaptor
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a sequence of examples, ignoring the annotations and the validation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    eventHandler: EventHandler? = nil
) async throws -> EstimatorToSupervisedAdaptor.Transformer where Input : Sequence, Input.Element == AnnotatedFeature
```

## Parameters 

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Return Value

The pre-defined transformer.

## See Also

### Fitting a transformer

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

typealias Transformer

The transformer type created by this estimator.

