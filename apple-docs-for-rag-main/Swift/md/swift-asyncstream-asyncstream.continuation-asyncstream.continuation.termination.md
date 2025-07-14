

- Swift
- AsyncStream
- AsyncStream.Continuation
-  AsyncStream.Continuation.Termination 

Enumeration

# AsyncStream.Continuation.Termination

A type that indicates how the stream terminated.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Termination
```

## Overview

The `onTermination` closure receives an instance of this type.

## Topics

### Termination States

case finished

The stream finished as a result of calling the continuation’s `finish` method.

case cancelled

The stream finished as a result of cancellation.

### Hashing

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing Termination Values

static func == (AsyncStream&lt;Element>.Continuation.Termination, AsyncStream&lt;Element>.Continuation.Termination) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Equatable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Hashable

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Sendable

## See Also

### Handling Termination

var onTermination: ((AsyncStream&lt;Element>.Continuation.Termination) -> Void)?

A callback to invoke when canceling iteration of an asynchronous stream.

