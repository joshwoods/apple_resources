

- Create ML Components
- UpdatableTabularEstimatorToSupervisedAdaptor
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes the transformer and optimizer to an encoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encodeWithOptimizer(
    _ transformer: UpdatableTabularEstimatorToSupervisedAdaptor.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

## Parameters 

`transformer`  

A transformer created by this estimator.

`encoder`  

An encoder.

## See Also

### Encoding and decoding

func encode(UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Reads the encoded transformer and optimizer.

