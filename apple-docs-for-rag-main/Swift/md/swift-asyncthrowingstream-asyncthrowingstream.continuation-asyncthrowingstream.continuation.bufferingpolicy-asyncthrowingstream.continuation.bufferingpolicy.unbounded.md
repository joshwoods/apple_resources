

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
- AsyncThrowingStream.Continuation.BufferingPolicy
-  AsyncThrowingStream.Continuation.BufferingPolicy.unbounded 

Case

# AsyncThrowingStream.Continuation.BufferingPolicy.unbounded

Continue to add to the buffer, treating its capacity as infinite.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case unbounded
```

## See Also

### Buffering Policies

case bufferingOldest(Int)

When the buffer is full, discard the newly received element.

case bufferingNewest(Int)

When the buffer is full, discard the oldest element in the buffer.

