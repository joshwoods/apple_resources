

- Create ML Components
- MLModelTransformerAdaptor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a transformation on a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> MLShapedArray
```

## Parameters 

`input`  

The input.

`eventHandler`  

An event handler.

## Return Value

The transformed input.

