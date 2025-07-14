

- Combine
- Publishers
- Publishers.Buffer
-  init(upstream:size:prefetch:whenFull:) 

Initializer

# init(upstream:size:prefetch:whenFull:)

Creates a publisher that buffers elements received from an upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    size: Int,
    prefetch: Publishers.PrefetchStrategy,
    whenFull: Publishers.BufferingStrategy.Failure>
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`size`  

The maximum number of elements to store.

`prefetch`  

The strategy for initially populating the buffer.

`whenFull`  

The action to take when the buffer becomes full.

