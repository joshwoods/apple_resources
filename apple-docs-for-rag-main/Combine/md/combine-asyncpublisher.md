

- Combine
-  AsyncPublisher 

Structure

# AsyncPublisher

A publisher that exposes its elements as an asynchronous sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AsyncPublisher where P : Publisher, P.Failure == Never
```

## Overview

`AsyncPublisher` conforms to AsyncSequence, which allows callers to receive values with the `for`-`await`-`in` syntax, rather than attaching a Subscriber.

Use the values property of the Publisher protocol to wrap an existing publisher with an instance of this type.

## Topics

### Creating an Asynchronous Publisher

init(P)

Creates a publisher that exposes elements received from an upstream publisher as an asynchronous sequence.

### Creating an Iterator

func makeAsyncIterator() -> AsyncPublisher&lt;P>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

The iterator that produces elements of the asynchronous publisher sequence.

### Supporting Types

typealias Element

The type of element produced by this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Asynchronous Publishers

struct AsyncThrowingPublisher

A publisher that exposes its elements as a throwing asynchronous sequence.

