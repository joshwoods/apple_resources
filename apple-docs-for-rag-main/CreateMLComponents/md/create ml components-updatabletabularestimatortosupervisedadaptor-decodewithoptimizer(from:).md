

- Create ML Components
- UpdatableTabularEstimatorToSupervisedAdaptor
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer and optimizer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> UpdatableTabularEstimatorToSupervisedAdaptor.Transformer
```

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

## See Also

### Encoding and decoding

func encode(UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

func decode(from: inout any EstimatorDecoder) throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

func encodeWithOptimizer(UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

