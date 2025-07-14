

- Create ML Components
- PreprocessingUpdatableSupervisedTemporalEstimator
-  encode(\_:to:) Deprecated

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func encode(
    _ transformer: PreprocessingUpdatableSupervisedTemporalEstimator.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Reads the encoded transformer and optimizer with a decoder.

Deprecated

func encodeWithOptimizer(PreprocessingUpdatableSupervisedTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

Deprecated

