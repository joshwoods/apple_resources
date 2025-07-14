

- Create ML Components
- LinearTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Scales a sequence of inputs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler? = nil
) -> [Element] where Element == S.Element, S : Sequence
```

## Parameters 

`input`  

A sequence of input values.

`eventHandler`  

An event handler.

## Return Value

An array of scaled values.

## See Also

### Performing the transformation

func applied(to: Element, eventHandler: EventHandler?) -> Element

Scales an input.

