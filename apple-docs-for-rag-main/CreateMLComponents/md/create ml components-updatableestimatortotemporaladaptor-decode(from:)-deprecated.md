

- Create ML Components
- UpdatableEstimatorToTemporalAdaptor
-  decode(from:) Deprecated

Instance Method

# decode(from:)

Decodes the transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> UpdatableEstimatorToTemporalAdaptor.Transformer
```

## See Also

### Encoding and decoding

func encode(UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

Deprecated

func encodeWithOptimizer(UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Reads the encoded transformer and optimizer with a decoder.

Deprecated

