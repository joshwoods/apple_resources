

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
-  AsyncThrowingStream.Continuation.YieldResult 

Enumeration

# AsyncThrowingStream.Continuation.YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum YieldResult
```

## Overview

The various `yield` methods of `AsyncThrowingStream.Continuation` return this type to indicate the success or failure of yielding an element to the continuation.

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

  Conforms when `Element` conforms to `Copyable`, `Element` conforms to `Escapable`, `Element` conforms to `Sendable`, and `Failure` conforms to `Error`.

## See Also

### Producing Elements

func yield(sending Element) -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

func yield(with: sending Result&lt;Element, Failure>) -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally or throw, based on a given result.

func yield() -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

