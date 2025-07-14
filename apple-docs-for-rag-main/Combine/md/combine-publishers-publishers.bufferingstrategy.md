

- Combine
- Publishers
-  Publishers.BufferingStrategy 

Enumeration

# Publishers.BufferingStrategy

A strategy that handles exhaustion of a buffer’s capacity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum BufferingStrategy where Failure : Error
```

## Topics

### Buffering Strategies

case dropNewest

When the buffer is full, discard the newly received element.

case dropOldest

When the buffer is full, discard the oldest element in the buffer.

case customError(() -> Failure)

When the buffer is full, execute the closure to provide a custom error.

## See Also

### Buffering Elements

func buffer(size: Int, prefetch: Publishers.PrefetchStrategy, whenFull: Publishers.BufferingStrategy&lt;Self.Failure>) -> Publishers.Buffer&lt;Self>

Buffers elements received from an upstream publisher.

enum PrefetchStrategy

A strategy for filling a buffer.

