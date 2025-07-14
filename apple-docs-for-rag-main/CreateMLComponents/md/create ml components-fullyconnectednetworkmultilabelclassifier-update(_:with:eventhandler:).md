

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a fully-connected network multi-label classifier model with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func update(
    _ transformer: inout FullyConnectedNetworkMultiLabelClassifierModel,
    with input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, InputSequence.Element == AnnotatedFeature, Set>
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Scalar` conforms to `Decodable`, `Scalar` conforms to `Encodable`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`transformer`  

A fully-connected network multi-label classifier model to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

