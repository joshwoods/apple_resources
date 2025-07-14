

- Swift
- AsyncStream
-  AsyncStream.Continuation 

Structure

# AsyncStream.Continuation

A mechanism to interface between synchronous code and an asynchronous stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Continuation
```

## Overview

The closure you provide to the `AsyncStream` in `init(_:bufferingPolicy:_:)` receives an instance of this type when invoked. Use this continuation to provide elements to the stream by calling one of the `yield` methods, then terminate the stream normally by calling the `finish()` method.

Note

Unlike other continuations in Swift, `AsyncStream.Continuation` supports escaping.

## Topics

### Producing Elements

func yield(sending Element) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

func yield(with: sending Result&lt;Element, Never>) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given result’s success value.

func yield() -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

enum YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

### Finishing the Stream

func finish()

Resume the task awaiting the next iteration point by having it return nil, which signifies the end of the iteration.

### Handling Termination

var onTermination: ((AsyncStream&lt;Element>.Continuation.Termination) -> Void)?

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

init(Element.Type, bufferingPolicy: AsyncStream&lt;Element>.Continuation.BufferingPolicy, (AsyncStream&lt;Element>.Continuation) -> Void)

Constructs an asynchronous stream for an element type, using the specified buffering policy and element-producing closure.

enum BufferingPolicy

A strategy that handles exhaustion of a buffer’s capacity.

