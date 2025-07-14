

- Create ML Components
- UniformRandomFloatingPointParameter
-  applied(to:generator:eventHandler:) 

Instance Method

# applied(to:generator:eventHandler:)

Performs the random apply operation on the input.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: RandomTransformer.Input,
    generator: inout some RandomNumberGenerator,
    eventHandler: EventHandler? = nil
) async throws -> RandomTransformer.Output
```

## Parameters 

`input`  

An input.

`generator`  

A random number generator.

`eventHandler`  

An event handler.

## Return Value

The randomly transformed image.

