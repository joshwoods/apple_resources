

- Create ML Components
- PreprocessingUpdatableSupervisedTabularEstimator
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer and optimizer with a decoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> PreprocessingUpdatableSupervisedTabularEstimator.Transformer
```

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

## See Also

### Encoding and decoding

func encode(PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

func encodeWithOptimizer(PreprocessingUpdatableSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

