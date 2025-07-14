

- Create ML Components
- SupervisedEstimator
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> Self.Transformer
```

**Required** Default implementation provided.

## Default Implementations

### SupervisedEstimator Implementations

func decode(from: inout any EstimatorDecoder) throws -> Self.Transformer

Decodes a previously fitted decodable transformer.

## See Also

### Encoding and decoding

func encode(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

**Required** Default implementation provided.

