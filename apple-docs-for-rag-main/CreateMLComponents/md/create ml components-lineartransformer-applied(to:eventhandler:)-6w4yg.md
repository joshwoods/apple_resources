

- Create ML Components
- LinearTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Scales an input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: Element,
    eventHandler: EventHandler? = nil
) -> Element
```

## Parameters 

`input`  

A floating-point value.

`eventHandler`  

An event handler.

## Return Value

A scaled value.

## See Also

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) -> [Element]

Scales a sequence of inputs.

