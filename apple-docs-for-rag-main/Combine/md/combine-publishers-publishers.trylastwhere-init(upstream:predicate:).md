

- Combine
- Publishers
- Publishers.TryLastWhere
-  init(upstream:predicate:) 

Initializer

# init(upstream:predicate:)

Creates a publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies an error-throwing predicate closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    predicate: @escaping (Publishers.TryLastWhere.Output) throws -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`predicate`  

The error-throwing closure that determines whether to publish an element.

