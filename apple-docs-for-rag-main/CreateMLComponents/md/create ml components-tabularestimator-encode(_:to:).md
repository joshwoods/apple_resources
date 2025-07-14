

- Create ML Components
- TabularEstimator
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: Self.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

**Required** Default implementation provided.

## Default Implementations

### TabularEstimator Implementations

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted encodable transformer.

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted transformer.

**Required** Default implementation provided.

