

- Create ML Components
- LogisticRegressionClassifier
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a logistic regression classifier model to a sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: Input,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> LogisticRegressionClassifierModel where Input : Sequence, Validation : Sequence, Input.Element == AnnotatedFeature, Label>, Validation.Element == AnnotatedFeature, Label>
```

## Parameters 

`input`  

A sequence of examples used for fitting the classifier.

`validation`  

A sequence of examples used for validating the fitted classifier.

`eventHandler`  

An event handler. This method reports accuracy metrics.

## Return Value

The fitted logistic regression classifier model.

## See Also

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifier&lt;Scalar, Label>.Transformer

Fits a logistic regression classifier model to a sequence of examples while validating with a validation sequence.

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

