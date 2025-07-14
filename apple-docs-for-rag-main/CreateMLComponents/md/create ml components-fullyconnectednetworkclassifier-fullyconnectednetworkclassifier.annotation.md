

- Create ML Components
- FullyConnectedNetworkClassifier
-  FullyConnectedNetworkClassifier.Annotation 

Type Alias

# FullyConnectedNetworkClassifier.Annotation

The annotation type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Annotation = Label
```

## See Also

### Fitting a classifier

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkClassifierModel&lt;Scalar, Label>

Fits a fully connected network classifier model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkClassifierModel&lt;Scalar, Label>

Fits a fully connected network classifier model to a sequence of examples.

typealias Transformer

The transformer type created by this estimator.

