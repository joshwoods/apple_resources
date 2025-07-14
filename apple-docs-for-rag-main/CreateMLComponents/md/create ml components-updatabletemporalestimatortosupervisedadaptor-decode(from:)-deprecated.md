

- Create ML Components
- UpdatableTemporalEstimatorToSupervisedAdaptor
-  decode(from:) Deprecated

Instance Method

# decode(from:)

Returns the pre-defined transformer.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> UpdatableTemporalEstimatorToSupervisedAdaptor.Transformer
```

## See Also

### Encoding and decoding

func encode(UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

Deprecated

func encodeWithOptimizer(UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Encodes the transformer and optimizer to an encoder.

Deprecated

func decodeWithOptimizer(from: inout any EstimatorDecoder) throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Reads the encoded transformer and optimizer with a decoder.

Deprecated

