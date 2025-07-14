

- Combine
- Publishers
- Publishers.Map
-  init(upstream:transform:) 

Initializer

# init(upstream:transform:)

Creates a publisher that transforms all elements from the upstream publisher with a provided closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    transform: @escaping (Upstream.Output) -> Output
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`transform`  

The closure that transforms elements from the upstream publisher.

