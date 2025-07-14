

- Create ML Components
- LinearRegressor
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout LinearRegressor.Transformer,
    with input: InputSequence,
    eventHandler: EventHandler?
) async throws where InputSequence : Sequence, InputSequence.Element == AnnotatedFeature, Scalar>
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

