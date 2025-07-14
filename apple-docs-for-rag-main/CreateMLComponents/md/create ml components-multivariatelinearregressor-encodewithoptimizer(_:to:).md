

- Create ML Components
- MultivariateLinearRegressor
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes the model and optimizer to an encoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func encodeWithOptimizer(
    _ model: MultivariateLinearRegressor.Model,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`model`  

A model this estimator creates.

`encoder`  

An encoder.

## See Also

### Encoding and decoding

func encode(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Decodes a previously fitted transformer.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Reads the encoded model and optimizer with a decoder.

