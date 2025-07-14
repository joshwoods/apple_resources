

- Combine
- Publishers
- Publishers.Contains
-  init(upstream:output:) 

Initializer

# init(upstream:output:)

Creates a publisher that emits a Boolean value when it receives a specific element from its upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    output: Upstream.Output
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`output`  

The element to match in the upstream publisher.

