

- Create ML Components
- TimeSeriesClassifier
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized model suitable for incremental fitting.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func makeTransformer() -> TimeSeriesClassifier.Model
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

