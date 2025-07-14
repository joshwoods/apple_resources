

- Swift
- AsyncStream
- AsyncStream.Continuation
-  AsyncStream.Continuation.YieldResult 

Enumeration

# AsyncStream.Continuation.YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum YieldResult
```

## Overview

The various `yield` methods of `AsyncStream.Continuation` return this type to indicate the success or failure of yielding an element to the continuation.

## Topics

### Yield Results

case enqueued(remaining: Int)

The stream successfully enqueued the element.

case dropped(Element)

The stream didn’t enqueue the element because the buffer was full.

case terminated

The stream didn’t enqueue the element because the stream was in a terminal state.

## Relationships

### Conforms To

- Sendable

  Conforms when `Element` conforms to `Copyable`, `Escapable`, and `Sendable`.

## See Also

### Producing Elements

func yield(sending Element) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

func yield(with: sending Result&lt;Element, Never>) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given result’s success value.

func yield() -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

