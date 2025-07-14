

- Create ML Components
- TransformerToEstimatorAdaptor
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Returns the pre-defined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: S,
    eventHandler: EventHandler? = nil
) async throws -> Transformer where S : Sequence, Transformer.Input == S.Element
```

## Parameters 

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Return Value

The pre-defined transformer.

