

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  FullyConnectedNetworkMultiLabelClassifier.Transformer 

Type Alias

# FullyConnectedNetworkMultiLabelClassifier.Transformer

The transformer type created by this estimator.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
typealias Transformer = FullyConnectedNetworkMultiLabelClassifierModel
```

## See Also

### Fitting a classifier

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>

Fits a fully-connected network multi-label classifier model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>

Fits a fully-connected network multi-label classifier model to a sequence of examples.

typealias Annotation

The annotation type.

