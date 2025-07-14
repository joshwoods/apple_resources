

- Create ML Components
- LogisticRegressionClassifier
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a logistic regression classifier model to a sequence of examples while validating with a validation sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    eventHandler: EventHandler? = nil
) async throws -> LogisticRegressionClassifier.Transformer where Input : Sequence, Input.Element == AnnotatedFeature, Label>
```

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifierModel&lt;Scalar, Label>

Fits a logistic regression classifier model to a sequence of examples.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

