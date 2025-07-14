

- Create ML Components
- ComposedTabularTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the composed transformation on a single input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws -> DataFrame
```

## Parameters 

`input`  

The transformer input.

`eventHandler`  

An event handler.

## Return Value

An output produced by applying the transformer to the input.

