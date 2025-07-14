

- Swift
- AsyncStream
- AsyncStream.Continuation
- AsyncStream.Continuation.YieldResult
-  AsyncStream.Continuation.YieldResult.terminated 

Case

# AsyncStream.Continuation.YieldResult.terminated

The stream didn’t enqueue the element because the stream was in a terminal state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case terminated
```

## Discussion

This indicates the stream terminated prior to calling `yield`, either because the stream finished normally or through cancellation.

## See Also

### Yield Results

case enqueued(remaining: Int)

The stream successfully enqueued the element.

case dropped(Element)

The stream didn’t enqueue the element because the buffer was full.

