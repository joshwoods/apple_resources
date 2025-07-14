

- Create ML Components
- TimeSeriesClassifier
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes the model and optimizer to an encoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func encodeWithOptimizer(
    _ transformer: TimeSeriesClassifier.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

