

- Combine
- Publishers
- Publishers.TryFilter
-  init(upstream:isIncluded:) 

Initializer

# init(upstream:isIncluded:)

Creates a publisher that republishes all elements that match a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    isIncluded: @escaping (Upstream.Output) throws -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`isIncluded`  

An error-throwing closure that indicates whether this filter should republish an element.

