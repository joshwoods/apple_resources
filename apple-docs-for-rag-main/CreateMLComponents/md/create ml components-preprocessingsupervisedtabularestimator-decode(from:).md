

- Create ML Components
- PreprocessingSupervisedTabularEstimator
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> PreprocessingSupervisedTabularEstimator.Transformer
```

## See Also

### Encoding and decoding

func encode(PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

