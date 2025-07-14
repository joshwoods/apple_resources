

- Create ML Components
- BoostedTreeRegressor
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> TreeRegressorModel
```

## See Also

### Encoding and decoding a regressor

func encode(TreeRegressorModel, to: inout any EstimatorEncoder) throws

Encodes a fitted transformer.

