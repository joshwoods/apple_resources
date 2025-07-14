

- Swift
- AsyncDropWhileSequence
- AsyncDropWhileSequence.Iterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Produces the next element in the drop-while sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(AsyncDropWhileSequence.Failure) -> Base.Element?
```

## Discussion

This iterator calls `next(isolation:)` on its base iterator and evaluates the result with the `predicate` closure. As long as the predicate returns `true`, this method returns `nil`. After the predicate returns `false`, for a value received from the base iterator, this method returns that value. After that, the iterator returns values received from its base iterator as-is, and never executes the predicate closure again.

