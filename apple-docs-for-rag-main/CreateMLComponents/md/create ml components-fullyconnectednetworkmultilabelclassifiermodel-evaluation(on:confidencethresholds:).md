

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifierModel
-  evaluation(on:confidenceThresholds:) 

Instance Method

# evaluation(on:confidenceThresholds:)

Computes evaluation metrics on annotated examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func evaluation(
    on input: some Collection, Set>>,
    confidenceThresholds: [Label : Float]
) throws -> MultiLabelClassificationMetrics
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`input`  

A collection of annotated examples.

`confidenceThresholds`  

A dictionary of label and confidence threshold pairs.

## Return Value

Multi-label classifier metrics.

