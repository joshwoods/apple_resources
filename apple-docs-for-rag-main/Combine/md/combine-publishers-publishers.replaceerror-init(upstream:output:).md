

- Combine
- Publishers
- Publishers.ReplaceError
-  init(upstream:output:) 

Initializer

# init(upstream:output:)

Creates a publisher that replaces any errors in the stream with a provided element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    output: Publishers.ReplaceError.Output
)
```

## Parameters 

`upstream`  

The element with which to replace errors from the upstream publisher.

`output`  

The publisher from which this publisher receives elements.

