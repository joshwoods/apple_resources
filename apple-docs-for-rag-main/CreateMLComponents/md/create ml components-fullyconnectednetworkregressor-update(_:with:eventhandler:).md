

- Create ML Components
- FullyConnectedNetworkRegressor
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a fully connected network regressor model with a new sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout FullyConnectedNetworkRegressorModel,
    with input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, InputSequence.Element == AnnotatedFeature, Float>
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`transformer`  

A fully connected network regressor model to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

