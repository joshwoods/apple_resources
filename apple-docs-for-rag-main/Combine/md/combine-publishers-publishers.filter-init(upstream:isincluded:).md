

- Combine
- Publishers
- Publishers.Filter
-  init(upstream:isIncluded:) 

Initializer

# init(upstream:isIncluded:)

Creates a publisher that republishes all elements that match a provided closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    isIncluded: @escaping (Upstream.Output) -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`isIncluded`  

A closure that indicates whether to republish an element.

