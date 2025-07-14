

- Swift
- TaskGroup
- TaskGroup.Iterator
-  next() 

Instance Method

# next()

Default implementation of `next()` in terms of `next(isolation:)`, which is required to maintain backward compatibility with existing async iterators.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next() async throws(Self.Failure) -> Self.Element?
```

