

- Create ML Components
- EstimatorToSupervisedAdaptor
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Does nothing since this estimator uses a pre-defined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: EstimatorToSupervisedAdaptor.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> EstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Returns the pre-defined transformer.

