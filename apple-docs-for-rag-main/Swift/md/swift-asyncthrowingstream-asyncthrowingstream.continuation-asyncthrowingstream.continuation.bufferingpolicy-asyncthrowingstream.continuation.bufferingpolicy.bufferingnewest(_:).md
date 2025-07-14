

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
- AsyncThrowingStream.Continuation.BufferingPolicy
-  AsyncThrowingStream.Continuation.BufferingPolicy.bufferingNewest(\_:) 

Case

# AsyncThrowingStream.Continuation.BufferingPolicy.bufferingNewest(\_:)

When the buffer is full, discard the oldest element in the buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case bufferingNewest(Int)
```

## Discussion

This strategy enforces keeping the specified amount of newest values.

## See Also

### Buffering Policies

case unbounded

Continue to add to the buffer, treating its capacity as infinite.

case bufferingOldest(Int)

When the buffer is full, discard the newly received element.

