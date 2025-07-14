

- Create ML Components
- OneHotEncoder
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a one-hot encoder to a sequence of categories.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: S,
    eventHandler: EventHandler? = nil
) throws -> OneHotEncoder.Transformer where S : Sequence, S.Element == Category?
```

## Parameters 

`input`  

A sequence of categories.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

