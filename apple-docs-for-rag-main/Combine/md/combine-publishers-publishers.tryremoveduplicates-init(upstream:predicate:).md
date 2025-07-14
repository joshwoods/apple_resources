

- Combine
- Publishers
- Publishers.TryRemoveDuplicates
-  init(upstream:predicate:) 

Initializer

# init(upstream:predicate:)

Creates a publisher that publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    predicate: @escaping (Publishers.TryRemoveDuplicates.Output, Publishers.TryRemoveDuplicates.Output) throws -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`predicate`  

An error-throwing closure to evaluate whether two elements are equivalent, for purposes of filtering. Return `true` from this closure to indicate that the second element is a duplicate of the first. If this closure throws an error, the publisher terminates with the thrown error.

