

- Create ML Components
- FullyConnectedNetworkRegressor
-  decode(from:) 

Instance Method

# decode(from:)

Decodes the estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> FullyConnectedNetworkRegressorModel
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`decoder`  

A decoder for the estimator.

## Return Value

A fully connected network regressor model.

