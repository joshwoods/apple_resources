

- Create ML Components
- PreprocessingUpdatableTemporalEstimator
-  encodeWithOptimizer(\_:to:) Deprecated

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes the transformer and optimizer to an encoder.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func encodeWithOptimizer(
    _ transformer: PreprocessingUpdatableTemporalEstimator.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

## Parameters 

`transformer`  

A transformer this estimator creates.

`encoder`  

An encoder.

## See Also

### Encoding and decoding

func encode(PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

Deprecated

func decode(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Decodes a previously fitted transformer.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> PreprocessingUpdatableTemporalEstimator&lt;Preprocessor, Estimator>.Transformer

Reads the encoded transformer and optimizer with a decoder.

Deprecated

