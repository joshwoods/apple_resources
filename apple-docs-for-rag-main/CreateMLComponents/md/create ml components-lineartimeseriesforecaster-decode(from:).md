

- Create ML Components
- LinearTimeSeriesForecaster
-  decode(from:) 

Instance Method

# decode(from:)

Decodes a previously fitted model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> LinearTimeSeriesForecaster.Transformer
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

