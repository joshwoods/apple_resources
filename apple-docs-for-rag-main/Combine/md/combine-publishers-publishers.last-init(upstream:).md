

- Combine
- Publishers
- Publishers.Last
-  init(upstream:) 

Initializer

# init(upstream:)

Creates a publisher that waits until after the stream finishes and then publishes the last element of the stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(upstream: Upstream)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

