

- Combine
- Publishers
- Publishers.TryAllSatisfy
-  init(upstream:predicate:) 

Initializer

# init(upstream:predicate:)

Returns a publisher that publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    predicate: @escaping (Upstream.Output) throws -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`predicate`  

A closure that evaluates each received element.

