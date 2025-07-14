

- Swift
- AsyncFilterSequence
- AsyncFilterSequence.Iterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Produces the next element in the filter sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(AsyncFilterSequence.Failure) -> Base.Element?
```

## Discussion

This iterator calls `next(isolation:)` on its base iterator; if this call returns `nil`, `next(isolation:)` returns nil. Otherwise, `next(isolation:)` evaluates the result with the `predicate` closure. If the closure returns `true`, `next(isolation:)` returns the received element; otherwise it awaits the next element from the base iterator.

