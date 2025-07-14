

- Swift
- AsyncIteratorProtocol
-  next(isolation:) 

Instance Method

# next(isolation:)

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(Self.Failure) -> Self.Element?
```

**Required** Default implementation provided.

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

## Default Implementations

### AsyncIteratorProtocol Implementations

func next(isolation: isolated (any Actor)?) async throws(Self.Failure) -> Self.Element?

Default implementation of `next(isolation:)` in terms of `next()`, which is required to maintain backward compatibility with existing async iterators.

