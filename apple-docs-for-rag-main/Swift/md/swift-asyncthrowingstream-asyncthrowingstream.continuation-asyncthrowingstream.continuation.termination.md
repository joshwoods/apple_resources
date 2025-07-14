

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
-  AsyncThrowingStream.Continuation.Termination 

Enumeration

# AsyncThrowingStream.Continuation.Termination

A type that indicates how the stream terminated.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Termination
```

## Overview

The `onTermination` closure receives an instance of this type.

## Topics

### Termination States

case finished(Failure?)

The stream finished as a result of calling the continuation’s `finish` method.

case cancelled

The stream finished as a result of cancellation.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling Termination

var onTermination: ((AsyncThrowingStream&lt;Element, Failure>.Continuation.Termination) -> Void)?

A callback to invoke when canceling iteration of an asynchronous stream.

