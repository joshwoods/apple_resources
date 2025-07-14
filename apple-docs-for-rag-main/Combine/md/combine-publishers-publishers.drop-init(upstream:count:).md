

- Combine
- Publishers
- Publishers.Drop
-  init(upstream:count:) 

Initializer

# init(upstream:count:)

Creates a publisher that omits a specified number of elements before republishing later elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    count: Int
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`count`  

The number of elements to drop.

