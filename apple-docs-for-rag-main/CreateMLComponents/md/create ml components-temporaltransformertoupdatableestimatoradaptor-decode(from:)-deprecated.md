

- Create ML Components
- TemporalTransformerToUpdatableEstimatorAdaptor
-  decode(from:) Deprecated

Instance Method

# decode(from:)

Returns the pre-defined transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> Transformer
```

## See Also

### Encoding and decoding

func encode(Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

Deprecated

func encodeWithOptimizer(Transformer, to: inout any EstimatorEncoder) throws

This method is part of the conformance. It doesn’t encode anything since the transformer is pre-defined, so don’t call it.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> Transformer

Returns the pre-defined transformer.

Deprecated

