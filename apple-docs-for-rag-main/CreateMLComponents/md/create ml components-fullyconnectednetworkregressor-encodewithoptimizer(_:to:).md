

- Create ML Components
- FullyConnectedNetworkRegressor
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes a fitted transformer with an optimizer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encodeWithOptimizer(
    _ transformer: FullyConnectedNetworkRegressor.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`transformer`  

A fully connected network regressor model.

`encoder`  

An encoder for the estimator.

