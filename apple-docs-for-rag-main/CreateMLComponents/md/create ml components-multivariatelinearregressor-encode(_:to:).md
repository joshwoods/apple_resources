

- Create ML Components
- MultivariateLinearRegressor
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func encode(
    _ model: MultivariateLinearRegressor.Model,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Decodes a previously fitted transformer.

func encodeWithOptimizer(MultivariateLinearRegressor&lt;Scalar>.Model, to: inout any EstimatorEncoder) throws

Encodes the model and optimizer to an encoder.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> MultivariateLinearRegressor&lt;Scalar>.Model

Reads the encoded model and optimizer with a decoder.

