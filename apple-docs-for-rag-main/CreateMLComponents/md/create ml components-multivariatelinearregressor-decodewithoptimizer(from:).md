

- Create ML Components
- MultivariateLinearRegressor
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded model and optimizer with a decoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor.Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded model.

## See Also

### Encoding and decoding

func encode(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Decodes a previously fitted transformer.

func encodeWithOptimizer(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes the model and optimizer to an encoder.

