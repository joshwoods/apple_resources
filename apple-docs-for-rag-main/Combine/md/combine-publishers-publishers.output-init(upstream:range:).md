

- Combine
- Publishers
- Publishers.Output
-  init(upstream:range:) 

Initializer

# init(upstream:range:)

Creates a publisher that publishes elements specified by a range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    range: CountableRange
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives its elements.

`range`  

The range of elements to publish.

