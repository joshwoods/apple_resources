

- Create ML Components
- TemporalTransformerToEstimatorAdaptor
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

