

- Create ML Components
- SupervisedTabularEstimator
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted encodable transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: Self.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Transformer` conforms to `Encodable`.

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted transformer.

**Required** Default implementation provided.

