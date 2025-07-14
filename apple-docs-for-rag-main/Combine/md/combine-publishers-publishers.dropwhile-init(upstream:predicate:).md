

- Combine
- Publishers
- Publishers.DropWhile
-  init(upstream:predicate:) 

Initializer

# init(upstream:predicate:)

Creates a publisher that omits elements from an upstream publisher until a given closure returns false.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    predicate: @escaping (Publishers.DropWhile.Output) -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`predicate`  

The closure that indicates whether to drop the element.

