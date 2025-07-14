

- Create ML Components
- UpdatableSupervisedEstimatorToTemporalAdaptor
-  encode(\_:to:) Deprecated

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func encode(
    _ transformer: UpdatableSupervisedEstimatorToTemporalAdaptor.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Decodes the transformer.

Deprecated

func encodeWithOptimizer(UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Reads the encoded transformer and optimizer with a decoder.

Deprecated

