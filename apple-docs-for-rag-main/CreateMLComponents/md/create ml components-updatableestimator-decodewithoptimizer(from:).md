

- Create ML Components
- UpdatableEstimator
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer and optimizer with a decoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> Self.Transformer
```

**Required**

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

## See Also

### Encoding and decoding

func encodeWithOptimizer(Self.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

**Required**

