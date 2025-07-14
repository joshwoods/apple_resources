

- Create ML Components
- EstimatorToSupervisedAdaptor
-  EstimatorToSupervisedAdaptor.Transformer 

Type Alias

# EstimatorToSupervisedAdaptor.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = Estimator.Transformer
```

## See Also

### Fitting a transformer

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples, ignoring the annotations and the validation.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

