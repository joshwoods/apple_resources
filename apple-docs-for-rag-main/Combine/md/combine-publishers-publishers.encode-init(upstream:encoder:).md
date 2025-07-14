

- Combine
- Publishers
- Publishers.Encode
-  init(upstream:encoder:) 

Initializer

# init(upstream:encoder:)

Creates a publisher that decodes elements received from an upstream publisher, using a given decoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    encoder: Coder
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`encoder`  

The encoder that decodes elements received from the upstream publisher.

