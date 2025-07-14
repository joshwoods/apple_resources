

- Create ML Components
- FullyConnectedNetworkRegressor
-  FullyConnectedNetworkRegressor.Transformer 

Type Alias

# FullyConnectedNetworkRegressor.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = FullyConnectedNetworkRegressorModel
```

## See Also

### Fitting a regressor

func fitted&lt;Input>(to: Input, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkRegressor&lt;Scalar>.Transformer

Fits a fully connected network regressor model to a sequence of examples.

func fitted&lt;Input, Validation>(to: Input, validateOn: Validation, eventHandler: EventHandler?) async throws -> FullyConnectedNetworkRegressorModel&lt;Scalar>

Fits a fully connected network regressor model to a sequence of examples.

typealias Annotation

The annotation type.

