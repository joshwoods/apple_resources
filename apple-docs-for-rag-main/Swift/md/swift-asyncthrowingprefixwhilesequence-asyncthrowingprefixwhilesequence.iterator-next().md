

- Swift
- AsyncThrowingPrefixWhileSequence
- AsyncThrowingPrefixWhileSequence.Iterator
-  next() 

Instance Method

# next()

Produces the next element in the prefix-while sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func next() async throws -> Base.Element?
```

## Discussion

If the predicate hasn’t failed yet, this method gets the next element from the base sequence and calls the predicate with it. If this call succeeds, this method passes along the element. Otherwise, it returns `nil`, ending the sequence. If calling the predicate closure throws an error, the sequence ends and `next()` rethrows the error.

