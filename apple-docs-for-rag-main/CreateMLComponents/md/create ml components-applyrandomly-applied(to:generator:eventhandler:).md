

- Create ML Components
- ApplyRandomly
-  applied(to:generator:eventHandler:) 

Instance Method

# applied(to:generator:eventHandler:)

Randomly applies a transformer on an input.

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

The input.

`generator`  

A random number generator.

`eventHandler`  

An event handler.

## Return Value

The randomly transformed input.

