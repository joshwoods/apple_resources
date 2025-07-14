

- Create ML Components
- TransformerToUpdatableEstimatorAdaptor
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Returns the pre-defined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> Transformer
```

## See Also

### Encoding and decoding

func encode(Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> Transformer

Returns the pre-defined transformer.

func encodeWithOptimizer(Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

