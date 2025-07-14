

- Swift
- AsyncStream
-  AsyncStream.Iterator 

Structure

# AsyncStream.Iterator

The asynchronous iterator for iterating an asynchronous stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Iterator
```

## Overview

This type doesn’t conform to `Sendable`. Don’t use it from multiple concurrent contexts. It is a programmer error to invoke `next()` from a concurrent context that contends with another such call, which results in a call to `fatalError()`.

## Topics

### Iterating over Elements

func next() async -> Element?

The next value from the asynchronous stream.

### Instance Methods

func next(isolation: isolated (any Actor)?) async -> Element?

The next value from the asynchronous stream.

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an Iterator

func makeAsyncIterator() -> AsyncStream&lt;Element>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

