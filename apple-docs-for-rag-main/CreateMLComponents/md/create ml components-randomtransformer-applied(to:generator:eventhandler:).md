

- Create ML Components
- RandomTransformer
-  applied(to:generator:eventHandler:) 

Instance Method

# applied(to:generator:eventHandler:)

Performs the random transformation on a single input.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: Self.Input,
    generator: inout some RandomNumberGenerator,
    eventHandler: EventHandler?
) async throws -> Self.Output
```

**Required**

## Parameters 

`input`  

The random transformer input.

`generator`  

A random number generator.

`eventHandler`  

An event handler.

## Return Value

An output produced by applying the random transformer to the input.

## See Also

### Performing the transformation

associatedtype Input

The input type.

**Required**

associatedtype Output

The output type.

**Required**

