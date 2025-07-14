

- Create ML Components
- TemporalEstimator
-  decode(from:) Deprecated

Instance Method

# decode(from:)

Decodes a previously fitted transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> Self.Transformer
```

**Required**

## See Also

### Encoding and decoding

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

**Required**

Deprecated

