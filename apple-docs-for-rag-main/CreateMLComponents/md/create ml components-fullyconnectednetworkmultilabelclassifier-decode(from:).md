

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  decode(from:) 

Instance Method

# decode(from:)

Decodes the estimator.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func decode(from decoder: inout any EstimatorDecoder) throws -> FullyConnectedNetworkMultiLabelClassifierModel
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Scalar` conforms to `Decodable`, `Scalar` conforms to `Encodable`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`decoder`  

A decoder for the estimator.

## Return Value

A fully-connected network multi-label classifier model.

