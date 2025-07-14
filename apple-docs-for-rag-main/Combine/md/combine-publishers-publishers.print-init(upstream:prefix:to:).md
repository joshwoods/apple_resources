

- Combine
- Publishers
- Publishers.Print
-  init(upstream:prefix:to:) 

Initializer

# init(upstream:prefix:to:)

Creates a publisher that prints log messages for all publishing events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    prefix: String,
    to stream: (any TextOutputStream)? = nil
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`prefix`  

A string with which to prefix all log messages.

