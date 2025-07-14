

- Combine
- Publishers
- Publishers.ReplaceEmpty
-  init(upstream:output:) 

Initializer

# init(upstream:output:)

Creates a publisher that replaces an empty stream with a provided element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    output: Publishers.ReplaceEmpty.Output
)
```

## Parameters 

`upstream`  

The element to deliver when the upstream publisher finishes without delivering any elements.

`output`  

The publisher from which this publisher receives elements.

