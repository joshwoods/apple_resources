

- Create ML Components
- FullyConnectedNetworkClassifier
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized fully connected network classifier model suitable for incremental fitting.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeTransformer() -> FullyConnectedNetworkClassifierModel
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

