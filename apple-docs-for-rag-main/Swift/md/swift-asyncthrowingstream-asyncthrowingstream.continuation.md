

- Swift
- AsyncThrowingStream
-  AsyncThrowingStream.Continuation 

Structure

# AsyncThrowingStream.Continuation

A mechanism to interface between synchronous code and an asynchronous stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Continuation
```

## Overview

The closure you provide to the `AsyncThrowingStream` in `init(_:bufferingPolicy:_:)` receives an instance of this type when invoked. Use this continuation to provide elements to the stream by calling one of the `yield` methods, then terminate the stream normally by calling the `finish()` method. You can also use the continuation’s `finish(throwing:)` method to terminate the stream by throwing an error.

Note

Unlike other continuations in Swift, `AsyncThrowingStream.Continuation` supports escaping.

## Topics

### Producing Elements

func yield(sending Element) -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

func yield(with: sending Result&lt;Element, Failure>) -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally or throw, based on a given result.

func yield() -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

enum YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

### Finishing the Stream

func finish(throwing: Failure?)

Resume the task awaiting the next iteration point by having it return nil, which signifies the end of the iteration.

### Handling Termination

var onTermination: ((AsyncThrowingStream&lt;Element, Failure>.Continuation.Termination) -> Void)?

A callback to invoke when canceling iteration of an asynchronous stream.

enum Termination

A type that indicates how the stream terminated.

### Enumerations

enum BufferingPolicy

A strategy that handles exhaustion of a buffer’s capacity.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a Continuation-Based Stream

init(Element.Type, bufferingPolicy: AsyncThrowingStream&lt;Element, Failure>.Continuation.BufferingPolicy, (AsyncThrowingStream&lt;Element, Failure>.Continuation) -> Void)

Constructs an asynchronous stream for an element type, using the specified buffering policy and element-producing closure.

enum BufferingPolicy

A strategy that handles exhaustion of a buffer’s capacity.

