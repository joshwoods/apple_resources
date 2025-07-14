

- Create ML Components
- PreprocessingUpdatableEstimator
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> PreprocessingUpdatableEstimator.Transformer
```

## See Also

### Encoding and decoding

func encode(PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer

Reads the encoded transformer and optimizer.

func encodeWithOptimizer(PreprocessingUpdatableEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

