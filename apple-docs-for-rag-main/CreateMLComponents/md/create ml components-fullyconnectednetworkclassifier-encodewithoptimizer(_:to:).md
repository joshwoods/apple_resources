

- Create ML Components
- FullyConnectedNetworkClassifier
-  encodeWithOptimizer(\_:to:) 

Instance Method

# encodeWithOptimizer(\_:to:)

Encodes a fitted transformer with an optimizer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encodeWithOptimizer(
    _ transformer: FullyConnectedNetworkClassifier.Transformer,
    to encoder: inout any EstimatorEncoder
) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`transformer`  

A fully connected network classifier model.

`encoder`  

An encoder for the estimator.

