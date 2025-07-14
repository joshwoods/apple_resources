

- Create ML Components
- ImageFlipper
-  callAsFunction(\_:eventHandler:) 

Instance Method

# callAsFunction(\_:eventHandler:)

Performs the transformation on a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func callAsFunction(
    _ input: S,
    eventHandler: EventHandler? = nil
) async throws -> [Self.Output] where S : Sequence, Self.Input == S.Element
```

## Parameters 

`input`  

The transformer inputs.

`eventHandler`  

An event handler.

## Return Value

The outputs produced by applying the transformer to the inputs.

