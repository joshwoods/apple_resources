

- Combine
- Publishers
- Publishers.MapError
-  init(upstream:transform:) 

Initializer

# init(upstream:transform:)

Creates a publisher that converts any failure from the upstream publisher into a new error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    transform: @escaping (Upstream.Failure) -> Failure
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`transform`  

The closure that converts the upstream failure into a new error.

## See Also

### Creating a Map Error Publisher

init(upstream: Upstream, (Upstream.Failure) -> Failure)

