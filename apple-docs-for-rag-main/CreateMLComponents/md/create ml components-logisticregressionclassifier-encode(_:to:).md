

- Create ML Components
- LogisticRegressionClassifier
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(
    _ transformer: LogisticRegressionClassifierModel,
    to encoder: inout any EstimatorEncoder
) throws
```

## See Also

### Encoding and decoding

func decode(from: inout any EstimatorDecoder) throws -> LogisticRegressionClassifierModel&lt;Scalar, Label>

Decodes a previously fitted transformer.

