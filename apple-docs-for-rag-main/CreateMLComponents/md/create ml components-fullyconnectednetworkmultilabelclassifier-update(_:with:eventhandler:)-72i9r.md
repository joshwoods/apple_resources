

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifier
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer on an async sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout Self.Transformer,
    with input: Input,
    eventHandler: EventHandler? = nil
) async throws where Input : AsyncSequence, Input.Element == AnnotatedFeature
```

## Parameters 

`transformer`  

A transformer to update.

`input`  

An async sequence of examples used for updating the transformer.

`eventHandler`  

An event handler.

## Discussion

Note that the async sequence is collected before updating the transformer.

