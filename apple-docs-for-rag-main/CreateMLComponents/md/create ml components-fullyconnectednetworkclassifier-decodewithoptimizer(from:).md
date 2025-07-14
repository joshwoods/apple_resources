

- Create ML Components
- FullyConnectedNetworkClassifier
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Decodes a previously fitted transformer with an optimizer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> FullyConnectedNetworkClassifier.Transformer
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`decoder`  

A decoder for the estimator.

## Return Value

A fully connected network classifier model.

