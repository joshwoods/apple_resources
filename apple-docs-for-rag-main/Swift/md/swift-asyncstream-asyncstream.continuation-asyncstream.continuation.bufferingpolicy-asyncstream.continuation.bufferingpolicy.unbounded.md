

- Swift
- AsyncStream
- AsyncStream.Continuation
- AsyncStream.Continuation.BufferingPolicy
-  AsyncStream.Continuation.BufferingPolicy.unbounded 

Case

# AsyncStream.Continuation.BufferingPolicy.unbounded

Continue to add to the buffer, without imposing a limit on the number of buffered elements.

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

