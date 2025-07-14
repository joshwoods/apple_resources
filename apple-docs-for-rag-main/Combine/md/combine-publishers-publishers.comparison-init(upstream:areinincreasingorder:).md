

- Combine
- Publishers
- Publishers.Comparison
-  init(upstream:areInIncreasingOrder:) 

Initializer

# init(upstream:areInIncreasingOrder:)

Creates a publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    areInIncreasingOrder: @escaping (Upstream.Output, Upstream.Output) -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives its elements.

`areInIncreasingOrder`  

A closure that receives two elements and returns true if they are in increasing order.

