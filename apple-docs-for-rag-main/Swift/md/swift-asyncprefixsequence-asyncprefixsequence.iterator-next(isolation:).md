

- Swift
- AsyncPrefixSequence
- AsyncPrefixSequence.Iterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Produces the next element in the prefix sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(AsyncPrefixSequence.Failure) -> Base.Element?
```

## Discussion

Until reaching the number of elements to include, this iterator calls `next(isolation:)` on its base iterator and passes through the result. After reaching the maximum number of elements, subsequent calls to `next(isolation:)` return `nil`.

