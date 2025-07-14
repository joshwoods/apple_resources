

- Combine
- Publishers
- Publishers.MapError
-  init(upstream:\_:) 

Initializer

# init(upstream:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    _ map: @escaping (Upstream.Failure) -> Failure
)
```

## See Also

### Creating a Map Error Publisher

init(upstream: Upstream, transform: (Upstream.Failure) -> Failure)

Creates a publisher that converts any failure from the upstream publisher into a new error.

