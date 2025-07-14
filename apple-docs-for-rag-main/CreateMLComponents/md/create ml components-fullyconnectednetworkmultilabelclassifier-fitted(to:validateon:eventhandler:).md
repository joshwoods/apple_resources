

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a fully-connected network multi-label classifier model to a sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func fitted(
    to input: Input,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> FullyConnectedNetworkMultiLabelClassifierModel where Input : Sequence, Validation : Sequence, Input.Element == AnnotatedFeature, Set>, Validation.Element == AnnotatedFeature, Set>
```

## Parameters 

`input`  

A sequence of examples used for fitting the classifier.

`validation`  

A sequence of examples used for validating the fitted multi-label classifier.

`eventHandler`  

An event handler.

## Return Value

The fitted fully-connected network multi-label classifier model.

## Discussion

The training process partitions the input into random batches according to the batch size configuration parameter. Training stops when the validation loss stops improving or when the maximum number of iterations is reached.

## See Also

### Fitting a classifier

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>

Fits a fully-connected network multi-label classifier model to a sequence of examples.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

