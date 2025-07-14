

- Create ML Components
- LinearTimeSeriesForecaster
-  encode(\_:to:) 

Instance Method

# encode(\_:to:)

Encodes a fitted model.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func encode(
    _ model: LinearTimeSeriesForecaster.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

