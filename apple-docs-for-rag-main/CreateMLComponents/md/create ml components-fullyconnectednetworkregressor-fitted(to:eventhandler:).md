

- Create ML Components
- FullyConnectedNetworkRegressor
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a fully connected network regressor model to a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    eventHandler: EventHandler? = nil
) async throws -> FullyConnectedNetworkRegressor.Transformer where Input : Sequence, Input.Element == AnnotatedFeature, Float>
```

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## Discussion

The training process partitions the input into random batches according to the batch size configuration parameter. Training stops when the maximum number of iterations is reached.

Note

This method does not do early-stopping, using a high value for `maximumIterations` may lead to over-fitting. Consider providing a validation set.

## See Also

### Fitting a regressor

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkRegressorModel&lt;Scalar>

Fits a fully connected network regressor model to a sequence of examples.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

