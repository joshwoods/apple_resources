

- Combine
- Publishers
- Publishers.PrefetchStrategy
-  Publishers.PrefetchStrategy.byRequest 

Case

# Publishers.PrefetchStrategy.byRequest

A strategy that avoids prefetching and instead performs requests on demand.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case byRequest
```

## Discussion

This strategy just forwards the downstream’s requests to the upstream publisher.

## See Also

### Prefetching Strategies

case keepFull

A strategy to fill the buffer at subscription time, and keep it full thereafter.

