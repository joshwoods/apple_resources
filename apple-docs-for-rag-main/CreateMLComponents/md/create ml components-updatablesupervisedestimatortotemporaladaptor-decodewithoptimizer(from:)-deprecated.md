

- Create ML Components
- UpdatableSupervisedEstimatorToTemporalAdaptor
-  decodeWithOptimizer(from:) Deprecated

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer and optimizer with a decoder.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> UpdatableSupervisedEstimatorToTemporalAdaptor.Transformer
```

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

## See Also

### Encoding and decoding

func encode(UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

Deprecated

func decode(from: inout any EstimatorDecoder) throws -> UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Decodes the transformer.

Deprecated

func encodeWithOptimizer(UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

Deprecated

