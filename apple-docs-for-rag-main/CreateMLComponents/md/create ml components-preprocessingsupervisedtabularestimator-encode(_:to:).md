

- Create ML Components
- PreprocessingSupervisedTabularEstimator
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: PreprocessingSupervisedTabularEstimator.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingSupervisedTabularEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

