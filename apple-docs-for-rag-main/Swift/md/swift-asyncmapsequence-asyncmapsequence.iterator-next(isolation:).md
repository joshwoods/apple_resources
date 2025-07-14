

- Swift
- AsyncMapSequence
- AsyncMapSequence.Iterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Produces the next element in the map sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(AsyncMapSequence.Failure) -> Transformed?
```

## Discussion

This iterator calls `next(isolation:)` on its base iterator; if this call returns `nil`, `next(isolation:)` returns `nil`. Otherwise, `next(isolation:)` returns the result of calling the transforming closure on the received element.

