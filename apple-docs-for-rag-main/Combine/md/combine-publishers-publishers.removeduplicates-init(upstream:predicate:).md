

- Combine
- Publishers
- Publishers.RemoveDuplicates
-  init(upstream:predicate:) 

Initializer

# init(upstream:predicate:)

Creates a publisher that publishes only elements that don’t match the previous element, as evaluated by a provided closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    predicate: @escaping (Publishers.RemoveDuplicates.Output, Publishers.RemoveDuplicates.Output) -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`predicate`  

A closure to evaluate whether two elements are equivalent, for purposes of filtering. Return `true` from this closure to indicate that the second element is a duplicate of the first.

