

- Create ML Components
- LogisticRegressionClassifier
-  LogisticRegressionClassifier.Annotation 

Type Alias

# LogisticRegressionClassifier.Annotation

The annotation type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Annotation = Label
```

## See Also

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifier&lt;Scalar, Label>.Transformer

Fits a logistic regression classifier model to a sequence of examples while validating with a validation sequence.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifierModel&lt;Scalar, Label>

Fits a logistic regression classifier model to a sequence of examples.

typealias Transformer

The transformer type created by this estimator.

