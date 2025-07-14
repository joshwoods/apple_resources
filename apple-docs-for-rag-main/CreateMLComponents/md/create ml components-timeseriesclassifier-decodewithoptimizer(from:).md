

- Create ML Components
- TimeSeriesClassifier
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded model and optimizer with a decoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> TimeSeriesClassifier.Transformer
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

