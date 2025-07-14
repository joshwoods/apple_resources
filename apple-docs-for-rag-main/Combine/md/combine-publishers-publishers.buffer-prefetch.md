

- Combine
- Publishers
- Publishers.Buffer
-  prefetch 

Instance Property

# prefetch

The strategy for initially populating the buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let prefetch: Publishers.PrefetchStrategy
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let size: Int

The maximum number of elements to store.

let whenFull: Publishers.BufferingStrategy&lt;Publishers.Buffer&lt;Upstream>.Failure>

The action to take when the buffer becomes full.

