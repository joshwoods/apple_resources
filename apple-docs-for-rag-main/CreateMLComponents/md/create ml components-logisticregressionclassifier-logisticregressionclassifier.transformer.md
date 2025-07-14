

- Create ML Components
- LogisticRegressionClassifier
-  LogisticRegressionClassifier.Transformer 

Type Alias

# LogisticRegressionClassifier.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = LogisticRegressionClassifierModel
```

## See Also

### Fitting

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifier&lt;Scalar, Label>.Transformer

Fits a logistic regression classifier model to a sequence of examples while validating with a validation sequence.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> LogisticRegressionClassifierModel&lt;Scalar, Label>

Fits a logistic regression classifier model to a sequence of examples.

typealias Annotation

The annotation type.

