

- Create ML Components
- EstimatorToSupervisedAdaptor
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a transformer to an async sequence of examples while validating with a validation sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    validateOn validation: Validation,
    eventHandler: EventHandler?
) async throws -> Self.Transformer where Input : AsyncSequence, Validation : Sequence, Input.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature
```

## Parameters 

`input`  

An async sequence of examples used for fitting the transformer.

`validation`  

A sequence of examples used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## Discussion

Note that the async sequence is collected before fitting the estimator. This may result in increased memory use. Consider using the update method to train progressively in batches.

