

- Swift
- AsyncIteratorProtocol
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func next() async throws -> Self.Element?
```

**Required** Default implementation provided.

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

## Default Implementations

### AsyncIteratorProtocol Implementations

func next() async throws(Self.Failure) -> Self.Element?

Default implementation of `next()` in terms of `next(isolation:)`, which is required to maintain backward compatibility with existing async iterators.

