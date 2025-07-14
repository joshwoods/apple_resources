

- Combine
- AsyncThrowingPublisher
- AsyncThrowingPublisher.Iterator
-  next() 

Instance Method

# next()

Produces the next element in the prefix sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func next() async throws -> P.Output?
```

## Return Value

The next published element, or nil if the publisher finishes normally. If the publisher terminates with an error, the call point receives the error as a `throw`.

