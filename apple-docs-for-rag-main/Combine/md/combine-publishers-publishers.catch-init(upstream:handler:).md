

- Combine
- Publishers
- Publishers.Catch
-  init(upstream:handler:) 

Initializer

# init(upstream:handler:)

Creates a publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    handler: @escaping (Upstream.Failure) -> NewPublisher
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives its elements.

`handler`  

A closure that accepts the upstream failure as input and returns a publisher to replace the upstream publisher.

