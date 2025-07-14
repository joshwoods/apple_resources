

- Create ML Components
- LogisticRegressionClassifier
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout LogisticRegressionClassifier.Transformer,
    with input: InputSequence,
    eventHandler: EventHandler?
) async throws where InputSequence : Sequence, InputSequence.Element == AnnotatedFeature, Label>
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

