

- Create ML Components
- ApplyEachRandomly
-  applied(to:generator:eventHandler:) 

Instance Method

# applied(to:generator:eventHandler:)

Applies each transformer randomly in order with a probability.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: Element,
    generator: inout some RandomNumberGenerator,
    eventHandler: EventHandler? = nil
) async throws -> Element
```

## Parameters 

`input`  

The input to the transformer.

`generator`  

A random number generator.

`eventHandler`  

An event handler.

## Return Value

The augmented input.

