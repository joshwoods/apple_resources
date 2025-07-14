

- Combine
- Publishers
- Publishers.PrefixUntilOutput
-  init(upstream:other:) 

Initializer

# init(upstream:other:)

Creates a publisher that republishes elements until another publisher emits an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    other: Other
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`other`  

Another publisher, the first output from which causes this publisher to finish.

