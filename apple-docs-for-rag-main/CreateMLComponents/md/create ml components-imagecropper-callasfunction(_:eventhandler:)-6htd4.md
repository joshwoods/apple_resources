

- Create ML Components
- ImageCropper
-  callAsFunction(\_:eventHandler:) 

Instance Method

# callAsFunction(\_:eventHandler:)

Performs the transformation on a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func callAsFunction(
    _ input: Self.Input,
    eventHandler: EventHandler? = nil
) async throws -> Self.Output
```

## Parameters 

`input`  

The transformer input.

`eventHandler`  

An event handler.

## Return Value

An output produced by applying the transformer to the input.

