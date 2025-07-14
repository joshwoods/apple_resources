

- Create ML Components
- LinearRegressor
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes the transformer and optimizer to an encoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func encodeWithOptimizer(
    _ transformer: LinearRegressorModel,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`transformer`  

A transformer this estimator creates.

`encoder`  

An encoder.

