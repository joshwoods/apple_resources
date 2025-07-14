

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
-  AsyncThrowingStream.Continuation.BufferingPolicy 

Enumeration

# AsyncThrowingStream.Continuation.BufferingPolicy

A strategy that handles exhaustion of a buffer’s capacity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum BufferingPolicy
```

## Topics

### Buffering Policies

case unbounded

Continue to add to the buffer, treating its capacity as infinite.

case bufferingOldest(Int)

When the buffer is full, discard the newly received element.

case bufferingNewest(Int)

When the buffer is full, discard the oldest element in the buffer.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a Continuation-Based Stream

init(Element.Type, bufferingPolicy: AsyncThrowingStream&lt;Element, Failure>.Continuation.BufferingPolicy, (AsyncThrowingStream&lt;Element, Failure>.Continuation) -> Void)

Constructs an asynchronous stream for an element type, using the specified buffering policy and element-producing closure.

struct Continuation

A mechanism to interface between synchronous code and an asynchronous stream.

