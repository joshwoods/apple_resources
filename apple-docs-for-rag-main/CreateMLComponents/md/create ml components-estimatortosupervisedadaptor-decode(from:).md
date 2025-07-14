

- Create ML Components
- EstimatorToSupervisedAdaptor
-  decode(from:) 

Instance Method

# decode(from:)

Returns the pre-defined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> EstimatorToSupervisedAdaptor.Transformer
```

## See Also

### Encoding and decoding

func encode(EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, to: inout any EstimatorEncoder) throws

Does nothing since this estimator uses a pre-defined transformer.

