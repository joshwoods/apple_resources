

- Create ML Components
- FullyConnectedNetworkRegressor
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Decodes a previously fitted transformer with an optimizer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> FullyConnectedNetworkRegressor.Transformer
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`decoder`  

A decoder for the estimator.

## Return Value

A fully connected network regressor model.

