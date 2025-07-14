

- Swift
- AsyncPrefixWhileSequence
- AsyncPrefixWhileSequence.Iterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Produces the next element in the prefix-while sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(AsyncPrefixWhileSequence.Failure) -> Base.Element?
```

## Discussion

If the predicate hasn’t yet failed, this method gets the next element from the base sequence and calls the predicate with it. If this call succeeds, this method passes along the element. Otherwise, it returns `nil`, ending the sequence.

