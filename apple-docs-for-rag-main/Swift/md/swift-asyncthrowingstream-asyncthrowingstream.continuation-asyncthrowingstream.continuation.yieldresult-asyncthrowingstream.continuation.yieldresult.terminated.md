

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
- AsyncThrowingStream.Continuation.YieldResult
-  AsyncThrowingStream.Continuation.YieldResult.terminated 

Case

# AsyncThrowingStream.Continuation.YieldResult.terminated

The stream didn’t enqueue the element because the stream was in a terminal state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case terminated
```

## Discussion

This indicates the stream terminated prior to calling `yield`, either because the stream finished normally or through cancellation, or it threw an error.

## See Also

### Yield Results

case enqueued(remaining: Int)

The stream successfully enqueued the element.

case dropped(Element)

The stream didn’t enqueue the element because the buffer was full.

