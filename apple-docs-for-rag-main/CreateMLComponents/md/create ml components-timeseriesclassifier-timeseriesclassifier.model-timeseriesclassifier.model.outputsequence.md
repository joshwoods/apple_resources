

- Create ML Components
- TimeSeriesClassifier
- TimeSeriesClassifier.Model
-  TimeSeriesClassifier.Model.OutputSequence 

Type Alias

# TimeSeriesClassifier.Model.OutputSequence

The output async sequence type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
typealias OutputSequence = AnyTemporalSequence>
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

