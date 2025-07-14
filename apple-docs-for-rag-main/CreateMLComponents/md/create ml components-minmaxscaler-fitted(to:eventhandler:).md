

- Create ML Components
- MinMaxScaler
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a min max scaler to a sequence of elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: S,
    eventHandler: EventHandler? = nil
) throws -> MinMaxScaler.Transformer where Element == S.Element, S : Sequence
```

## Parameters 

`input`  

A sequence of elements.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

