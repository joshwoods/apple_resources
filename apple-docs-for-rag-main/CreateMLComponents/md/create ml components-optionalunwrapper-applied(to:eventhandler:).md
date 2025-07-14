

- Create ML Components
- OptionalUnwrapper
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Unwraps an optional element or throws if the value is `nil`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to input: Element?,
    eventHandler: EventHandler? = nil
) throws -> Element
```

## Parameters 

`input`  

The optional input.

`eventHandler`  

An event handler.

## Return Value

The unwrapped value.

## Discussion

Throws

`MissingValueError` if the input is `nil`.

