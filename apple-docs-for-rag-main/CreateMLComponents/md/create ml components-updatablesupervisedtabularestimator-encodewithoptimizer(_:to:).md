

- Create ML Components
- UpdatableSupervisedTabularEstimator
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes the transformer and optimizer to an encoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encodeWithOptimizer(
    _ transformer: Self.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

**Required**

## Parameters 

`transformer`  

A transformer this estimator creates.

`encoder`  

An encoder.

## See Also

### Encoding and decoding

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> Self.Transformer

Reads the encoded transformer and optimizer with a decoder.

**Required**

