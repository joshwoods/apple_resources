

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized fully-connected network multi-label classifier model suitable for incremental fitting.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func makeTransformer() -> FullyConnectedNetworkMultiLabelClassifierModel
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Scalar` conforms to `Decodable`, `Scalar` conforms to `Encodable`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

