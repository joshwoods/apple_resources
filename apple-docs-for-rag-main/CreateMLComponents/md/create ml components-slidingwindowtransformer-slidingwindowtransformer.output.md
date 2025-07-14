

- Create ML Components
- SlidingWindowTransformer
-  SlidingWindowTransformer.Output 

Type Alias

# SlidingWindowTransformer.Output

The output type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Output = [Input]
```

## See Also

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> SlidingWindowTransformer&lt;Input>.WindowSequence

Extracts a window sequence from the input sequence

typealias Input

The input type.

struct WindowSequence

An async sequence of windows.

