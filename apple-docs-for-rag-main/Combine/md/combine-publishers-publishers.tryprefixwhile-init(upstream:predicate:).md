

- Combine
- Publishers
- Publishers.TryPrefixWhile
-  init(upstream:predicate:) 

Initializer

# init(upstream:predicate:)

Creates a publisher that republishes elements while an error-throwing predicate closure indicates publishing should continue.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    predicate: @escaping (Publishers.TryPrefixWhile.Output) throws -> Bool
)
```

## Parameters 

`upstream`  

The publisher from which this publisher receives elements.

`predicate`  

The error-throwing closure that determines whether publishing should continue.

