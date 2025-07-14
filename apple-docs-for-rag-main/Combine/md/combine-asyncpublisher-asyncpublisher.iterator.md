

- Combine
- AsyncPublisher
-  AsyncPublisher.Iterator 

Structure

# AsyncPublisher.Iterator

The iterator that produces elements of the asynchronous publisher sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Iterator
```

## Topics

### Iterating over Elements

func next() async -> P.Output?

Produces the next element in the prefix sequence.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an Iterator

func makeAsyncIterator() -> AsyncPublisher&lt;P>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

