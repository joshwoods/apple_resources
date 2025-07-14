

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
- AsyncThrowingStream.Continuation.YieldResult
-  AsyncThrowingStream.Continuation.YieldResult.dropped(\_:) 

Case

# AsyncThrowingStream.Continuation.YieldResult.dropped(\_:)

The stream didn’t enqueue the element because the buffer was full.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case dropped(Element)
```

## Discussion

The associated element for this case is the element that the stream dropped.

## See Also

### Yield Results

case enqueued(remaining: Int)

The stream successfully enqueued the element.

case terminated

The stream didn’t enqueue the element because the stream was in a terminal state.

