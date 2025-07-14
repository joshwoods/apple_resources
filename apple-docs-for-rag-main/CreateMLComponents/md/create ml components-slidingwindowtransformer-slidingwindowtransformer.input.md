

- Create ML Components
- SlidingWindowTransformer
-  SlidingWindowTransformer.Input 

Type Alias

# SlidingWindowTransformer.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Input = Input
```

## See Also

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> SlidingWindowTransformer&lt;Input>.WindowSequence

Extracts a window sequence from the input sequence

typealias Output

The output type.

struct WindowSequence

An async sequence of windows.

